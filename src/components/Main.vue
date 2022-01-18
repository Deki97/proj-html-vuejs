<template>
    <main>
        <Services />

        <About />

        <ActionsProjects />

        <ProcessManagement />
    </main>
</template>


<script>
import Services from './Services.vue';
import About from './About.vue';
import ActionsProjects from './ActionsProjects.vue';
import ProcessManagement from './ProcessManagement.vue';

export default {
    name: 'Main',
    components: {
        Services,
        About,
        ActionsProjects,
        ProcessManagement
    }
}
</script>


<style lang="scss" scoped>

</style>