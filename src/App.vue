<script>

    import AppHeader from './components/AppHeader.vue'
    import AppBulletPoint from './components/AppBulletPoint.vue'
    import AppAbout from './components/AppAbout.vue'
    import AppProjects from './components/AppProjects.vue'
    import AppProcess from './components/AppProcess.vue'
    import AppFeedback from './components/AppFeedback.vue'

    export default {
        components: {
            AppHeader,
            AppBulletPoint,
            AppAbout,
            AppProjects,
            AppProcess,
            AppFeedback
        }
    }

</script>

<template>
    <AppHeader></AppHeader>
    <main>
        <AppBulletPoint></AppBulletPoint>
        <AppAbout></AppAbout>
        <AppProjects></AppProjects>
        <AppProcess></AppProcess>
        <AppFeedback></AppFeedback>
    </main>

</template>

<style lang="scss">

    @use './style/generic';
    @use './style/partials/variables' as *;

</style>