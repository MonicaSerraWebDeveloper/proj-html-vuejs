<script>

    export default {
        name: 'AppProcess'
    }

</script>

<template>
    <section class="container-elements">
        <div class="title-container">
            <div class="container">
                <div class="row">
                    <h4>How it works in practise</h4>
                    <h2><span class="span-title">Process</span> Management</h2>
                    <p>We work with innovative methodologies to ensure that the entire reformatting process is done from start to finish as planned</p>
                </div>
            </div>
        </div>
        <div class="process-container">
            <div class="container-large">
                <div class="row">
                    <div class="col-20 single-process-container">
                        <span>01</span>
                        <h3>Collection of information</h3>
                        <p>Lorem ipsum dolor sit amet consectetur.</p>
                    </div> 
                    <div class="col-20 single-process-container">
                        <span>02</span>
                        <h3>Strategic planning</h3>
                        <p>Lorem ipsum dolor sit amet consectetur.</p>
                    </div>
                    <div class="col-20 single-process-container">
                        <span>03</span>
                        <h3>Assignment of responsibilities</h3>
                        <p>Lorem ipsum dolor sit amet consectetur.</p>
                    </div>
                    <div class="col-20 single-process-container">
                        <span>04</span>
                        <h3>Formatting process</h3>
                        <p>Lorem ipsum dolor sit amet consectetur.</p>
                    </div>
                    <div class="col-20 single-process-container">
                        <span>05</span>
                        <h3>Continuity formalization</h3>
                        <p>Lorem ipsum dolor sit amet consectetur.</p>
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
        text-align: center;

        .title-container {
            padding-bottom: 100px;
            border-bottom: 2px solid $primary-color;

            .container {
                max-width: 700px;
                
                .row {
                    flex-direction: column;
                    align-items: center;
                    gap: 12px;
                }
            }            
        }

        .process-container {
            position: relative;
            padding-bottom: 100px;

            .row {
                justify-content: space-evenly;
                position: absolute;
                top: -25px;
                left: 10%;
                right: 10%;

                .col-20 {
                    width: calc(100% / 5);
                }

                .single-process-container {
                    display: flex;
                    flex-direction: column;
                    align-items: center;
                    gap: 12px;

                    span {
                        color: $primary-color;
                        background-color: $bg-color;
                        border-radius: 50%;
                        width: 50px;
                        height: 50px;
                        line-height: 50px;
                        font-size: 18px;
                    }

                    h3 {
                        line-height: 22px;
                    }
                }
            }
        }

    }

    


</style>