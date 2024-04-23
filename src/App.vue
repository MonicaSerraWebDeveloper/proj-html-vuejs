<script>

    import AppHeader from './components/AppHeader.vue'
    import AppBulletPoint from './components/AppBulletPoint.vue'
    import AppAbout from './components/AppAbout.vue'
    import AppProjects from './components/AppProjects.vue'

    export default {
        components: {
            AppHeader,
            AppBulletPoint,
            AppAbout,
            AppProjects
        }
    }

</script>

<template>
    <AppHeader></AppHeader>
    <main>
        <AppBulletPoint></AppBulletPoint>
        <AppAbout></AppAbout>
        <AppProjects></AppProjects>
    </main>

</template>

<style lang="scss">

    @use './style/generic';
    @use './style/partials/variables' as *;



</style>