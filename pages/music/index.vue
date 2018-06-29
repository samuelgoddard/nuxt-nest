<template>
  <section class="wrapper">
    <h1>Music</h1>
    <p>async data example</p>
    <nav class="m-nav">
      <nuxt-link v-for="(music, index) in music" :key="index" class="nav-item nav-item--underlined nav-item--chevron" :to="{ name: 'music-id', params: { id: music.id } }">{{ music.title }}</nuxt-link>
    </nav>
  </section>
</template>

<script>
import axios from 'axios'

export default {
  // Get the data
  asyncData({ req, params }) {
    // We can return a Promise instead of calling the callback
    return axios.get('https://jsonplaceholder.typicode.com/posts')
      .then((res) => {
        return { music: res.data.slice(0, 8) }
      })
  },
  head: {
    title: 'Music'
  }
}
</script>