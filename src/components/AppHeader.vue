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
            <div class="container">
                <div class="row">
                    <div class="col-50">
                        <h4>Human Resources</h4>
                        <h1>Get More Productivity</h1>
                        <p>Planning, recruitment and selection process and performance evaluation of employees.</p>
                        <div class="container-button">
                            <button class="button-primary">
                                Get in touch
                            </button>
                            <button class="button-secondary-negative ">
                                Read More
                            </button>
                        </div>
                    </div>
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
        position: relative;
        background-image: url('../assets/img/bg-4.jpg');
        background-position: top;
        background-size: cover;
        background-repeat: no-repeat;
        color: $white;

        &::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 1;
            background-color: $woodsmoke;
            opacity: 0.5;
        }    

        .row {
            width: 100%;
            padding: 20px 0;
            align-items: center;     
            z-index: 10;
            
            & > * {
                z-index: 10;
            }

            .logo {
                flex-grow: 1;
                font-size: 22px;
                letter-spacing: 6px;
                font-weight: 500;
                text-transform: uppercase;

                .span-bg-logo {
                    color: $primary-color;
                    background-color: $transparent-primary;
                    padding: 4px 0;
                    padding-left: 24px;
                    border-top-left-radius: 20px;
                    border-bottom-left-radius: 20px;
                }
            }

            nav {
                ul {
                display: flex;
                gap: 20px;
                font-weight: 400;
                text-transform: uppercase;

                    .active {
                        color: $primary-color;
                    }
                }

            }

            .col-50 {
                width: calc(100% / 2);
                padding: 100px 0;
                display: flex;
                flex-direction: column;
                gap: 30px;
                
                p {
                    color: $white;
                }

                .container-button {
                    display: flex;
                    gap: 10px;
                }

            }
        }
    }

</style>