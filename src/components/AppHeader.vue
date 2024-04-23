<script>

    export default {
        name: 'AppHeader'
    }


</script>

<template>

    <header>
        <div class="top-bar-header">
            <div class="container">
                <div class="row text-small gap">
                    <div class="grow"><i class="fa-solid fa-clock padding-r-l"></i> Open Hours: Mon - Sat - 9:00 - 18:00</div>
                    <div><i class="fa-solid fa-phone padding-r-l"></i> +1(305) 1234-5678</div>
                    <div><i class="fa-solid fa-envelope padding-r-l"></i> hello@example.com</div>
                    <div class="container-social">
                        <i class="fa-brands fa-facebook-f"></i>
                        <i class="fa-brands fa-twitter"></i>
                        <i class="fa-brands fa-linkedin-in"></i>
                    </div>
                </div>
            </div>
        </div>
        <div class="menu-container">
            <div class="container">
                <div class="row">
                    
                </div>
            </div>
        </div>
    </header>

</template>

<style scoped lang="scss">

    @use '../style/partials/buttons' as *;
    @use '../style/partials/variables' as *;

    .top-bar-header {
        background-color: $darkblue;
        color: #fff;
        
        .row {
            padding: 8px 0;
            width: 100%;

            .padding-r-l {
                padding: 0 6px;
            }

            .grow {
                flex-grow: 1;
            }

            .container-social {
                display: flex;
                gap: 26px;
                align-items: center;
            }
        }
    }
</style>