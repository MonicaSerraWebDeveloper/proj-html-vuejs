<script>

    export default {
        name: 'AppFooter',
        props: {
            listFooterData: Object
        }
    }

</script>

<template>

    <div class="footer-container">
        <div class="container">
            <div class="row">
                <div class="left-side">
                    <div class="title-side-left-container">
                        <h4>Send a message</h4>
                        <h2>Get in <span class="span-title-negative">Touch</span></h2>
                        <p>We will respond to your message as soon as possible</p>
                    </div>
                    <div class="form-container">
                        <input class="width-50" type="text" placeholder="Name">
                        <input class="width-50" type="email" placeholder="Email" name="" id="">
                        <input class="width-50" type="number" placeholder="Phone" name="" id="">
                        <select class="width-50" name="" id="">
                            <option value="">More Info</option>
                        </select>
                        <textarea name="" id="" placeholder="Message" cols="100" rows="5"></textarea>
                    </div>
                    <button class="button-primary">Send</button>
                </div>
                <div class="right-side">
                    <h3>Example Inc.</h3>
                    <p>Lorem ipsum dolor sit amet consectetur.</p>
                    <p>Lorem ipsum dolor sit amet consectetur.</p>
                    <div class="info-container">
                        <i class="fa-solid fa-phone"></i>
                        <span>{{ listFooterData.phone }}</span>
                    </div>
                    <div class="info-container">
                        <i class="fa-solid fa-envelope"></i>
                        <span>{{ listFooterData.email }}</span>
                    </div>
                    <div class="info-container">
                        <i class="fa-solid fa-location-dot"></i>
                        <span>{{ listFooterData.address }}</span>
                    </div>
                    <button class="button-secondary-negative">View map</button>
                </div>
            </div>
        </div>
    </div>
    <div class="bottom-footer">
        <div class="container">
            <div class="row">
                <div>Copyright</div>
                <div>© 2024 - Classe-122</div>
            </div>
        </div>
        
    </div>

</template>

<style scoped lang="scss">

    @use '../style/partials/variables' as *;
    @use '../style/partials/buttons' as *;

    .footer-container {
        background-color: $woodsmoke;
        padding: 100px 0;

        .row {
            gap: 50px;

            .left-side {
                width: calc(70% - 25px);

                .title-side-left-container {
                    padding-bottom: 50px;

                    h2 {
                        color: $white;
                    }

                    & > * {
                        padding: 12px 0;
                    }
                }

                
                .form-container {
                    display: flex;
                    flex-wrap: wrap;
                    gap: 10px;
                    padding-bottom: 26px;

                    & > * {
                        background-color: #1d1d23;
                        border: 1px solid #1d1d23;
                        border-radius: 4px;
                        padding: 0 12px;
                        color: $abbey;
                        outline: none;
                        font-family: "Kanit", sans-serif;
                    }

                    select {
                        color: $abbey;
                        padding: 0 10px;
                    }

                    .width-50 {
                        width: calc((100% / 2) - 10px);
                        height: 36px;
                        
                    }

                    textarea {
                        margin-right: 10px;
                        padding-top: 12px;
                    }
                }
            }

            .right-side {
                width: calc(30% - 25px);

                h3 {
                    color: $white;
                }

                p {
                    color: $white;
                }

                & > *:not(:last-child) {
                    padding-bottom: 12px;
                }

                .info-container {
                    color: $darker-primary;
                    display: flex;
                    align-items: center;
                    gap: 10px;
                    font-weight: 200;

                    i {
                        color: $darker-primary;
                        width: 34px;
                        height: 34px;
                        border-radius: 50%;
                        text-align: center;
                        line-height: 34px;
                        background-color: #0f2128;
                    }
                }

            }
            
        }
    }

    .bottom-footer {
        background-color: #000;
        height: 80px;
        color: $white;
        font-size: 14px;
        font-weight: 200;

        .container {
            height: 100%;
            width: 100%;
        }

        .row {
            height: 100%;
            width: 100%;
            align-items: center;
            justify-content: space-between;

        }
    }


</style>