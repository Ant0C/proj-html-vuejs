<script>
</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col-description">
                <ul>
                    <li class="motto">CORPORATE & WEDDINGS</li>
                    <li class="title">
                        <h2>Baking Special Moments</h2>
                    </li>
                </ul>
            </div>
            <div class="col-img">
                <div class="card_img">
                    <img src="/img/corporate-bg.jpg" alt="ok">
                    <img class="img" src="/img/corporate-hover-bg.jpg" alt="ok">
                    <div class="info_img">
                        <div class="motto">International Bakery</div>
                        <div class="title">
                            <h2>Corporate Events</h2>
                        </div>
                        <a class="button" href="#">Explore More</a>
                    </div>
                </div>
                <div class="card_img">
                    <img src="/img/wedding-bg.jpg" alt="ok">
                    <img class="img" src="/img/wedding-hover-bg.jpg" alt="ok">
                    <div class="info_img">
                        <div class="motto">Private dining hall</div>
                        <div class="title">
                            <h2>Wenddings & Parties</h2>
                        </div>
                        <a class="button" href="#">Explore More</a>
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
    flex-direction: column;
    text-align: center;

    .col-description {


        .motto {
            color: #878589;
            font-size: 15px;
            font-family: 'Roboto', sans-serif;
            font-weight: 300;
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
    }



    .col-img {
        display: flex;
        flex-direction: row;
        gap: 6rem;

        img {
            width: 750px;
        }

        .card_img {
            position: relative;
        }

        .info_img {
            opacity: 0;
            position: absolute;
            top: 40%;
            bottom: 0;
            left: 0;
            right: 0;

            .title {
                color: #ffffff;
                font-size: 25px;
                margin-top: 15px;
                margin-bottom: 40px;
            }

            .motto {
                color: #ffffff;
                font-size: 15px;
                font-family: 'Roboto', sans-serif;
                font-weight: 300;
            }

            .button {
                width: 40%;
                padding: 15px 25px;
                color: #ffffff;
                font-size: 18px;
                background-color: #5b2ca2;
                text-align: center;
                border-radius: 6px;
                font-family: 'Roboto', sans-serif;
                font-weight: 300;
            }
        }

        .img {
            opacity: 0;
            position: absolute;
            top: 0;
            bottom: 0;
            left: 0;
            right: 0;
            transition: all .8s;
        }

        .card_img:hover {

            .img {
                opacity: 1;
            }

            .info_img {
                opacity: 1;

                .button:hover {
                    transition: all .2s;
                    color: #5b2ca2;
                    background-color: #ffffff;
                }
            }
        }
    }
}
</style>
