<template>
    <main>
        <Services />

        <About />
    </main>
</template>


<script>
import Services from './Services.vue';
import About from './About.vue';

export default {
    name: 'Main',
    components: {
        Services,
        About
    }
}
</script>


<style lang="scss" scoped>

</style>