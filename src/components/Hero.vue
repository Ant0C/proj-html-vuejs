<script>

export default {
    data() {
        return {}
    }
}
</script>

<template>
    <div class="hero">
        <div class="container">
            <div class="row">
                <div class="col-hero">
                    <div class="motto">FRESH & TASTY BAKERY EVERY DAY</div>
                    <div class="title">
                        <h2>The Perfect Fresh Bread</h2>
                    </div>
                    <div class="description">
                        Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius.
                        Aliquam erat volutpat.
                        Nullam quis sagittis nibh ac nulla id orci tempor.
                    </div>
                    <div class="button">
                        <a href="#">
                            Explore our products
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../src/style/general.scss' as *;

.hero {
    background-image: url(/img/hero-header-bakery.jpg);
    background-position: center center;
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
    top: -200px;
    z-index: -1;
    height: 900px;


    .container {
        max-width: 1600px;
        margin: 0 auto;

    }

    .row {
        display: flex;
        font-family: 'Source Serif Pro', serif;
        font-weight: 400;

        .col-hero {
            flex-basis: 30%;
            margin-top: 200px;
            position: relative;
            top: 200px;

            .motto {
                color: #878589;
                font-size: 18px;
                font-family: 'Roboto', sans-serif;
                font-weight: 300;
            }

            .title {
                color: #5b2ca2;
                font-size: 35px;
                margin-top: 10px;
                margin-bottom: 15px;
            }

            .description {
                color: #878589;
                font-size: 18px;
                line-height: 1.5;
                margin-bottom: 30px;
            }

            .button {
                width: 45%;
                padding: 10px 15px 10px 15px;
                color: #5b2ca2;
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
            }
        }
    }
}
</style>
