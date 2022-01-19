<template>
    <main>
        <Services />

        <About />

        <ActionsProjects />

        <ProcessManagement />

        <Feedback />
    </main>
</template>


<script>
import Services from './Services.vue';
import About from './About.vue';
import ActionsProjects from './ActionsProjects.vue';
import ProcessManagement from './ProcessManagement.vue';
import Feedback from './Feedback.vue';

export default {
    name: 'Main',
    components: {
        Services,
        About,
        ActionsProjects,
        ProcessManagement,
        Feedback
    }
}
</script>


<style lang="scss" scoped>

</style>