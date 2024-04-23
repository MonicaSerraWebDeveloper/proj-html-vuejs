<script>

    export default {
        name: 'AppAbout'
    }

</script>

<template>

    <div class="container-about">
        <div class="container">
            <div class="row">
                <div class="col-50 padding-text">
                    <h4>About the Network</h4>
                    <h2><span class="span-title">The</span> Company</h2>
                    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Non alias voluptas, hic tempore minus sed? Et quas a molestiae ea?</p>
                    <div class="data-container">
                        <div class="single-data">
                            <span>0</span>
                            <h3>Employees</h3>
                            <p>Lorem ipsum dolor sit amet.</p>
                        </div>
                        <div class="single-data">
                            <span>0</span>
                            <h3>Partners</h3>
                            <p>Lorem ipsum dolor sit amet.</p>
                        </div>
                        <div class="single-data">
                            <span>0</span>
                            <h3>Customers</h3>
                            <p>Lorem ipsum dolor sit amet.</p>
                        </div>
                    </div>
                    <div class="button-container">
                        <button class="button-primary"> Get in Touch</button>
                        <button class="button-secondary">Read More</button>
                    </div>
                </div>
                <div class="col-50">
                    <img src="../assets/img/about-5.jpg" alt="">
                </div>
            </div>
        </div>
    </div>

</template>

<style scoped lang="scss">
    @use '../style/partials/variables' as *;
    @use '../style/partials/buttons' as *;

    
    .container-about {
        position: relative;

        .container {
            display: flex;

            .padding-text > * {
                    padding: 12px 0;
                }

            .col-50 {
                width: calc(100% / 2);
                padding: 100px 0;

                .data-container {
                    display: flex;

                    .single-data {
                        width: calc(100% / 3);

                        span {
                            color: $primary-color;
                            font-size: 25px;
                            padding-left: 20px;
                            font-weight: 500;
                        }
                    }
                }

                img {
                    position: absolute;
                    top: 0;
                    right: 0;
                    width: 50%;
                    height: 100%;
                    object-fit: cover;
                }

                .button-container {
                    display: flex;
                    gap: 10px;
                }

            }

        }

        
    }

</style>