<script>

    export default {
        name: 'AppProjects'
    }

</script>

<template>

    <section class="container-projects">
        <div class="container">
            <div class="row">
                <div class="title-container">
                    <h4>We do more for everyone</h4>
                    <h2>Actions & <span class="span-title-negative">Projects</span></h2>
                </div>
                <div class="category-projects">
                    <ul>
                        <a href="#"><li class="active">All</li></a>
                        <a href="#"><li>Institutional</li></a>
                        <a href="#"><li>Social</li></a>
                        <a href="#"><li>Events</li></a>
                        <a href="#"><li>Innovation</li></a>
                        <a href="#"><li>Evironment</li></a>
                        <a href="#"><li>Technology</li></a>
                    </ul>
                    <div class="grid-container">
                        <div class="col-33">
                            <div class="card">
                                <img src="../assets/img/project-1.jpg" alt="">
                                <h3>Academic professional program in social media</h3>
                            </div>
                        </div>
                        <div class="col-33">
                            <div class="card">
                                <img src="../assets/img/project-2.jpg" alt="">
                                <h3>President's speech at the annual meeting</h3>
                            </div>
                        </div>
                        <div class="col-33">
                            <div class="card">
                                <img src="../assets/img/project-3.jpg" alt="">
                                <h3>International business trip in Shanghai</h3>
                            </div>
                        </div>
                        <div class="col-33">
                            <div class="card">
                                <img src="../assets/img/project-4.jpg" alt="">
                                <h3>Technology workshop with education theme</h3>
                            </div>
                        </div>
                        <div class="col-33">
                            <div class="card">
                                <img src="../assets/img/project-5.jpg" alt="">
                                <h3>Donation of clothes and food to the partner NGO</h3>
                            </div>
                        </div>
                        <div class="col-33">
                            <div class="card">
                                <img src="../assets/img/project-6.jpg" alt="">
                                <h3>Confraternization of the procurement team</h3>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

</template>

<style scoped lang="scss">

    @use '../style/partials/variables' as *;
    
    .container-projects {
        background-color: $woodsmoke;
        padding: 100px 0;

        .row {
            flex-direction: column;
            align-items: center;

            .title-container {
                text-align: center;

                & > * {
                    padding: 12px;
                }

                h2 {
                    color: $white;
                }

            }
            ul {
                display: flex;
                justify-content: space-evenly;
                text-transform: uppercase;
                padding: 20px;

                li {
                    padding: 6px;

                    &:hover {
                        color: $white;
                        background-color: $transparent-primary;
                        border-radius: 4px;
                        padding: 6px;
                    }
                }

                .active {
                    color: $white;
                    background-color: $transparent-primary;
                    border-radius: 4px;
                    padding: 6px;
                }
            }

            .category-projects {
                width: 100%;

                .grid-container {
                    display: flex;
                    flex-wrap: wrap;
                    gap: 20px;

                    .col-33 {
                        width: calc((100% / 3) - 20px);

                        .card {
                            width: 100%;
                            height: 300px;
                            position: relative;
                            display: flex;
                            align-items: flex-end;
                            cursor: pointer;
                            background-color: $woodsmoke;

                            img {
                                position: absolute;
                                top: 0;
                                left: 0;
                                width: 100%;
                                height: 100%;
                                border-radius: 10px;
                                object-fit: cover;
                                opacity: 0.5;
                            }


                            h3 {
                                color: $white;
                                line-height: 20px;
                                text-align: center;
                                z-index: 10;
                            }
                        }
                    }
                }
            }
        }
    }

</style>