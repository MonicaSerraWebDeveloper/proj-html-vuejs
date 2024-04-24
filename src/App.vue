<script>

    import AppHeader from './components/AppHeader.vue'
    import AppBulletPoint from './components/AppBulletPoint.vue'
    import AppAbout from './components/AppAbout.vue'
    import AppProjects from './components/AppProjects.vue'
    import AppProcess from './components/AppProcess.vue'
    import AppFeedback from './components/AppFeedback.vue'
    import AppFooter from './components/AppFooter.vue'

    export default {
        components: {
            AppHeader,
            AppBulletPoint,
            AppAbout,
            AppProjects,
            AppProcess,
            AppFeedback,
            AppFooter
        },

        data() {
            return {

                // Creaiamo i nostri data per popolare l'Header e il footer con un Object "Data" in cui sono contenute due chiavi "menu" che è un Array di Oggetti e "contacts" che è un Oggetto.
                data: {
                    menu: [
                    {
                        text: 'home',
                        active: false
                    },
                    {
                        text: 'about',
                        active: false
                    },
                    {
                        text: 'project',
                        active: false
                    },
                    {
                        text: 'process',
                        active: true
                    },
                    {
                        text: 'testimonials',
                        active: false
                    }
                ],
                contacts: {
                    email: 'hello@example.com',
                    phone: '+1(305) 1234-5678',
                    address: 'Main Avenue, 987',
                }
                }
            }
        }
    }

</script>

<template>
    <AppHeader :listMenu="data"></AppHeader>
    <main>
        <AppBulletPoint></AppBulletPoint>
        <AppAbout></AppAbout>
        <AppProjects></AppProjects>
        <AppProcess></AppProcess>
        <AppFeedback></AppFeedback>
    </main>
    <AppFooter :listFooterData="data.contacts"></AppFooter>
</template>

<style lang="scss">

    @use './style/generic';
    @use './style/partials/variables' as *;

</style>