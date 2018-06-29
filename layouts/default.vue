<template>
    <div>
        <!-- Nav component -->
        <Nav/>
        <!-- Nuxt render area -->
        <nuxt/>
    </div>
</template>

<script>
import Nav from '~/components/Nav.vue'

export default {
    components: {
        Nav
    }
}
</script>