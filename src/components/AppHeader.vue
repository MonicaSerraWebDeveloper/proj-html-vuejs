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
                <div class="row gap text">
                    <div class="logo"> <span class="span-bg-logo">Nex</span>gen</div>
                    <nav>
                        <ul class="list-menu">
                            <a href="#"><li>Home</li></a>
                            <a href="#"><li>About</li></a>
                            <a href="#"><li>Project</li></a>
                            <a href="#"><li class="active">Process</li></a>
                            <a href="#"><li>Testimonials</li></a>
                        </ul>
                    </nav>
                    <i class="fa-regular fa-user"></i>
                    <button class="button-primary">Get in touch</button>
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

    .menu-container {
        background-image: url('../assets/img/bg-4.jpg');
        // height: 800px;
        color: $white;
        text-transform: uppercase;

        .row {
            width: 100%;
            padding: 20px 0;
            align-items: center;

            .logo {
                flex-grow: 1;
                font-size: 22px;
                letter-spacing: 6px;
                font-weight: 500;

                .span-bg-logo {
                    color: $primary-color;
                    background-color: $transparent-primary;
                    padding: 4px 0;
                    padding-left: 24px;
                    border-top-left-radius: 20px;
                    border-bottom-left-radius: 20px;
                }
            }

            ul {
                display: flex;
                gap: 20px;
                font-weight: 400;

                .active {
                    color: $primary-color;
                }
            }
        }
    }

</style>