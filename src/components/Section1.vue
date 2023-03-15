<script>
</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col-description">
                <div class="motto">OUR PRODUCTS</div>
                <div class="title">
                    <h2>All our delectable pastries are backed fresh in our Kitchen very morning, and are made with
                        all-natural, all organic ingredients.</h2>
                </div>
                <a href="#" class="button">Buy Avada Today!</a>
            </div>
            <div class="col-img">
                <a href="#">
                    <img class="img_card" src="/img/choco-chip-cookies-500x638.jpg" alt="ok">
                    <div class="info_product">
                        <h3 class="name-product">Choco Chip Cookies</h3>
                        <p class="type-product">Cookies, Pastries</p>
                        <p class="price-product">$18.00 - $32.00</p>
                    </div>
                </a>
            </div>
            <div class="col-img">
                <a href="#">
                    <img class="img_card" src="/img/strawberry-jam-cookies-500x638.jpg" alt="ok">
                    <div class="info_product">
                        <h3 class="name-product">Strawberry Jam Cookies</h3>
                        <p class="type-product">Cookies, Pastries</p>
                        <p class="price-product">$36.00 - $60.00</p>
                    </div>
                </a>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../src/style/general.scss' as *;

.container {
    max-width: 1600px;
    margin: 0 auto;
    margin-top: -50px;
}

.row {
    display: flex;

    gap: 15px;

    .col-description,
    .col-img {
        flex-basis: calc(100%*(4/12));
    }

    .col-description {
        margin-right: 50px;

        .motto {
            color: #878589;
            font-size: 18px;
            font-family: 'Roboto', sans-serif;
            font-weight: 300;
        }

        .title {
            color: #554599;
            font-size: 24px;
            margin-top: 15px;
            margin-bottom: 40px;
        }

        .button {
            width: 40%;
            padding: 10px 20px;
            color: #ffffff;
            font-size: 18px;
            background-color: #5b2ca2;
            text-align: center;
            border-radius: 6px;
            font-family: 'Roboto', sans-serif;
            font-weight: 300;
        }

        .button:hover {
            transition: all .2s;
            color: #5b2ca2;
            background-color: #ffffff;
            border: 1px solid #e9dedc
        }
    }

    .col-img {
        position: relative;

        .info_product {
            opacity: 0;
            font-family: 'Roboto', sans-serif;
            font-weight: 300;
            position: absolute;
            text-align: center;
            color: #ffffff;
            top: 40%;
            left: 30%;

            .name-product {
                color: #ffffff;
                font-size: 22px;
            }

            .price-product {
                color: #ffffff;
                font-size: 30px;
            }

            .type-product {
                color: #ffffff;
                font-size: 15px;
                font-family: 'Roboto', sans-serif;
                font-weight: 300;
                margin-top: 20px;
                margin-bottom: 20px;
            }

        }
    }

    .col-img:hover {
        .img_card {
            filter: saturate(0.4) hue-rotate(18deg) brightness(0.7);
            transition: all .8s;
        }

        .info_product {
            opacity: 1;
        }

    }
}
</style>
