<template>
    <div class="">
        <TheNav />
        <nuxt />
        <TheFooter />
        <TheSignoff />
    </div>
</template>

<style lang="postcss">
    h1, h2, h3{
        @apply font-display
    }
</style>

<script>
import Logo from '~/components/old-style/Logo.vue'
import TheNav from '~/components/old-style/TheNav.vue'
import TheFooter from '~/components/old-style/TheFooter.vue'
import TheSignoff from '~/components/old-style/TheSignoff.vue'

export default {
    layout: 'customPage',
    components: {
        Logo,
        TheNav,
        TheFooter,
        TheSignoff
    },
    scrollToTop: true
}
</script>