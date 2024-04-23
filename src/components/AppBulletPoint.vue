<script>

    export default {
        name: 'AppBulletPoint'
    }

</script>

<template>
    <div class="bullet-point-container">
        <div class="container">
            <div class="row">
                <div class="col-33">
                    <div class="card">
                        <i class="fa-solid fa-user-group"></i>
                        <h3>Human Capital</h3>
                        <p>Humanizing business Harness the power of technology to improve the way people work</p>
                    </div>
                </div>
                <div class="col-33">
                    <div class="card">
                        <i class="fa-solid fa-chart-pie"></i>
                        <h3>Core Business</h3>
                        <p>It takes innovative approches to transform, modernize, and run axisting platforms</p>
                    </div>
                </div>
                <div class="col-33">
                    <div class="card">
                        <i class="fa-solid fa-gauge-high"></i>
                        <h3>Performance</h3>
                        <p>Achieving maximum impact and value from investiments in finance and supply chain</p>
                    </div>
                </div>

            </div>
        </div>
    </div>

</template>

<style scoped lang="scss">

    @use '../style/generic';
    @use '../style/partials/variables' as *;

   
    .bullet-point-container {
        background-color: $greynurse;
        padding: 100px 0;
        
        .row {
            gap: 20px;
                .col-33 {
                width: calc((100% / 3) - 20px);

                .card > * {
                    padding: 12px 0;
                }
                .card {

                    i {
                        font-size: 20px;
                        padding: 14px;
                        border-radius: 50%;
                        color: $primary-color;
                        background-color: #daeced;
                    
                    }
                }
                
            }

        }
        
    
    }


</style>