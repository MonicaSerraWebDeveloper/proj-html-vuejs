<script>

    import AppHeader from './components/AppHeader.vue'
    import AppBulletPoint from './components/AppBulletPoint.vue'

    export default {
        components: {
            AppHeader,
            AppBulletPoint
        }
    }

</script>

<template>
    <AppHeader></AppHeader>
    <main>
        <AppBulletPoint></AppBulletPoint>
    </main>

</template>

<style lang="scss">

    @use './style/generic';
    @use './style/partials/variables' as *;



</style>