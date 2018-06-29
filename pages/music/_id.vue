<template>
  <section class="wrapper">
    <div class="g">
      <div class="g__col g__col-12 g__col-8@medium">
        <nuxt-link class="nav-item nav-item--underlined" to="/music">Back to all music</nuxt-link>
        <h1>{{ post.title }}</h1>
        <p>{{ post.body }}</p>
      </div>
    </div>
  </section>
</template>

<script>
import axios from 'axios'

export default {
  // Get the data
  async asyncData({ params }) {
    // We can use async/await ES6 feature
    let { data } = await axios.get(`https://jsonplaceholder.typicode.com/posts/${params.id}`)
    return { post: data }
  },
  // Meta stuff / page title
  head() {
    return {
      title: this.post.title
    }
  }
}
</script>