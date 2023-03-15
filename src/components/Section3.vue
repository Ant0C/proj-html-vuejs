<script>
</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col-description">
                <ul>
                    <li class="title">
                        <h2>Find a freshly baked product perfect for you</h2>
                    </li>
                    <li class="description">
                        Integer a nibh vitae ex porttitor rutrum et ut velit. Etiam ac felis at leo feugiat placerat. Sed ac
                        nulla id orci tempor convallis sed.
                    </li>
                    <li class="button"> <a href="#">Shop All Products</a></li>
                </ul>
            </div>
            <div class="col-carousel">
                <div class="carousel_cards">
                    <div>
                        <div class="card">
                            <img class="img_card" src="/img/choco-chip-cookies-600x765.jpg" alt="ok">
                            <span class="info_card">SELECT OPTIONS / QUICK VIEW</span>
                        </div>
                        <h3 class="name-product">Choco Chip Cookies</h3>
                        <p class="price-product">$18.00 - $32.00</p>
                    </div>
                    <div>
                        <div class="card">
                            <img class="img_card" src="/img/strawberry-jam-cookies-600x765.jpg" alt="ok">
                            <span class="info_card">SELECT OPTIONS / QUICK VIEW</span>
                        </div>
                        <h3 class="name-product">Strawberry Jam Cookies</h3>
                        <p class="price-product">$36.00 - $60.00</p>
                    </div>
                    <div>
                        <div class="card">
                            <img class="img_card" src="/img/strawberry-donut-600x765.jpg" alt="ok">
                            <span class="info_card">SELECT OPTIONS / QUICK VIEW</span>
                        </div>
                        <h3 class="name-product">Strawberry Donut</h3>
                        <p class="price-product">$24.00 - $48.00</p>
                    </div>
                    <div>
                        <div class="card">
                            <img class="img_card" src="/img/perfect-macarons-600x765.jpg" alt="ok">
                            <span class="info_card">SELECT OPTIONS / QUICK VIEW</span>
                        </div>
                        <h3 class="name-product">Perfect Macarons</h3>
                        <p class="price-product">$32.00 - $56.00</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../src/style/general.scss' as *;

.container {
    max-width: 1600px;
    margin: 0 auto;
    margin-top: 200px;
}

.row {
    display: flex;
    align-items: center;

    .col-description {
        flex-basis: 30%;
        margin-right: 20px;

        ul {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
        }

        .description {
            color: #878589;
            font-size: 20px;
            margin-bottom: 30px;
        }


        .title {
            color: #5b2ca2;
            font-size: 25px;
            margin-top: 15px;
            margin-bottom: 40px;
        }

        .button {
            width: 40%;
            padding: 10px;
            color: #ffffff;
            font-size: 18px;
            background-color: #5b2ca2;
            text-align: center;
            border-radius: 6px;
            font-family: 'Roboto', sans-serif;
            font-weight: 300;
        }

        .button:hover {
            color: #5b2ca2;
            background-color: #e9dedc;
            transition: all .2s;
        }
    }

    .col-carousel {
        flex-basis: 70%;

        .carousel_cards {
            display: flex;
            gap: 10px;
            text-align: center;

            .info_card {
                display: none;
            }

            .card {
                position: relative;
            }

            .card:hover {

                .img_card {
                    filter: saturate(0.4) hue-rotate(18deg) brightness(0.7);
                    transition: all .2s;
                }

                .info_card {
                    display: inline-block;
                    font-family: 'Roboto', sans-serif;
                    font-weight: 300;
                    position: absolute;
                    color: #ffffff;
                    top: 50%;
                    left: 8%;
                }
            }

            .name-product {
                color: #5b2ca2;
                font-size: 22px;
                margin-top: 15px;
                margin-bottom: 20px;
            }

            .price-product {
                color: #878589;
                font-size: 15px;
            }
        }
    }
}
</style>
