<script>

    export default {
        name: 'AppFeedback'
    }

</script>

<template>

    <section class="container-elements">
        <div class="title-container">
            <div class="container-small">
                <div class="row">
                    <h4>Customer Testimonials</h4>
                    <h2>Trusted <span class="span-title">Feedback</span></h2>
                    <p>We work intensively in search of ideals that can add up in the lives of our customers. This is what moves us and we are greatful for the recognition.</p>
                </div>
            </div>
            
        </div>
        <div class="card-container">
            <div class="container">
                <div class="row">
                    <div class="col-33">
                        <div class="card">
                            <img src="../assets/img/logo-1.png" alt="">
                            <p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed voluptatum consequatur quas veniam provident aliquam iste eum quaerat.    
                            Distinctio deserunt quaerat maxime, voluptas harum possimus.
                            </p>
                            <i class="fa-solid fa-quote-right"></i>
                        </div>
                    </div>
                    <div class="col-33">
                        <div class="card">
                            <img src="../assets/img/logo-2.png" alt="">
                            <p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed voluptatum consequatur quas veniam provident aliquam iste eum quaerat.    
                            Distinctio deserunt quaerat maxime, voluptas harum possimus.
                            </p>
                            <i class="fa-solid fa-quote-right"></i>
                        </div>
                    </div>
                    <div class="col-33">
                        <div class="card">
                            <img src="../assets/img/logo-3.png" alt="">
                            <p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed voluptatum consequatur quas veniam provident aliquam iste eum quaerat.    
                            Distinctio deserunt quaerat maxime, voluptas harum possimus.
                            </p>
                            <i class="fa-solid fa-quote-right"></i>
                        </div>
                    </div>
                </div>
            </div>
            
        </div>
    </section>

</template>

<style scoped lang="scss">

    @use '../style/partials/variables' as *;

    .container-elements {
        padding: 100px 0;
        background-color: $greynurse;

        .title-container {
            padding-bottom: 50px;

            .row {
                flex-direction: column;
                align-items: center;
                text-align: center;

                & > * {
                    padding: 12px 0;
                }
            }
        }
        
        .card-container {

            .row {
                gap: 20px;

                .col-33 {
                    width: calc((100% / 3) - 20px );

                    .card {
                        position: relative;
                        padding: 34px;

                        img {
                            width: 100px;
                        }

                        i {
                            position: absolute;
                            bottom: 16px;
                            right: 16px;
                            font-size: 26px;
                            color: $silversand;
                        }
                    }
                }
            }
        }
    }

</style>