<template>
  <div class="wrapper p-bottom--double@medium">
    <nav class="m-nav m-nav--horizontal">
      <!-- 
      Loop through the nuxt generated router items
      (https://nuxtjs.org/guide/routing) 
      -->
      <nuxt-link class="nav-item" v-for="route in $router.options.routes.slice().reverse()" :key="route.name" :to="route.path" v-if="!/\:/.test(route.path)" >{{ route.name }}</nuxt-link>
    </nav>
  </div>
</template>
