<script>
</script>

<template>
    <div class="banner">
        <div class="row">
            <div class="col-banner">
                <div>
                    <div class="motto">TRY OUR SEASONAL PRODUCTS</div>
                    <div class="title">
                        <h2>Order for pick-up or delivery to your home</h2>
                    </div>
                    <a href="#" class="button">Shop Now</a>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../src/style/general.scss' as *;

.banner {
    background-image: url(/img/call-to-action-bg.jpg);
    background-position: center center;
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
    height: 540px;
    margin-top: 200px;

    .row {
        display: flex;
        font-family: 'Source Serif Pro', serif;
        font-weight: 400;

        .col-banner {
            flex-basis: 46%;
            margin-top: 200px;
            margin-left: 200px;

            .motto {
                color: #878589;
                font-size: 18px;
                font-family: 'Roboto', sans-serif;
                font-weight: 300;
            }

            .title {
                color: #ffffff;
                font-size: 40px;
                margin-top: 10px;
                margin-bottom: 50px;
            }

            .button {
                width: 15%;
                padding: 15px 20px;
                color: #282d2c;
                font-size: 18px;
                background-color: white;
                text-align: center;
                border-radius: 6px;
                font-family: 'Roboto', sans-serif;
                font-weight: 300;
            }

            .button:hover {
                color: #ffffff;
                background-color: #5b2ca2;
                transition: all .2s;
            }
        }
    }
}
</style>
