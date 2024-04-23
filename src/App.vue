<script>

    import AppHeader from './components/AppHeader.vue'
    import AppBulletPoint from './components/AppBulletPoint.vue'
    import AppAbout from './components/AppAbout.vue'
    import AppProjects from './components/AppProjects.vue'
    import AppProcess from './components/AppProcess.vue'

    export default {
        components: {
            AppHeader,
            AppBulletPoint,
            AppAbout,
            AppProjects,
            AppProcess
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
    </main>

</template>

<style lang="scss">

    @use './style/generic';
    @use './style/partials/variables' as *;

</style>