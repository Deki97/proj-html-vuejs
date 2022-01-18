<template>
    <main>
        <Services />

        <About />

        <ActionsProjects />
    </main>
</template>


<script>
import Services from './Services.vue';
import About from './About.vue';
import ActionsProjects from './ActionsProjects.vue';

export default {
    name: 'Main',
    components: {
        Services,
        About,
        ActionsProjects
    }
}
</script>


<style lang="scss" scoped>

</style>