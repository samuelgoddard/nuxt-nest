<template>
  <nav class="m-nav m-nav--horizontal">
    <!-- 
    Loop through the nuxt generated router items
    (https://nuxtjs.org/guide/routing) 
    -->
    <nuxt-link class="nav-item" v-for="route in $router.options.routes" :key="route.name" :to="route.path">{{route.name}}</nuxt-link>
  </nav>
</template>
