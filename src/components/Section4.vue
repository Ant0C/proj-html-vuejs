<script>
</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col-card01">
                <div class="title_card">
                    <h3 class="title">Tell us what you have in mind</h3>
                    <p class="number">01</p>
                </div>
                <div class="info_card">
                    <p class="motto">MANUAL INGREDIENTS SELECTION</p>
                    <p class="description">
                        Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius. Ut eu laoreet ex.
                        Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec
                        lorem erat, finibus in velit placerat, rutrum augue.
                    </p>
                </div>
            </div>
            <div class="col-card02">
                <div class="title_card">
                    <h3 class="title">We Start Baking</h3>
                    <p class="number">02</p>
                </div>
                <div class="info_card">
                    <p class="motto">SWEET & DELICIOUS</p>
                    <p class="description">
                        Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius. Ut eu laoreet ex.
                        Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec
                        lorem erat, finibus in velit placerat.
                    </p>
                </div>
            </div>
            <div class="col-card03">
                <div>
                    <p class="motto">DONT JUST TAKE OUR WORD FOR IT</p>
                    <h3 class="title">
                        “Finally found an alternative to the mass produced products. Something that incorporates real
                        organic ingredients, nutrient dense wellness while promoting sustainability and activity.”
                    </h3>
                    <p class="motto">
                        Rachel Cooper, Founder
                    </p>
                </div>
            </div>
            <div class="col-card04">
                <div class="title_card">
                    <h3 class="title">Delivered to your home</h3>
                    <p class="number">03</p>
                </div>
                <div class="info_card">
                    <p class="motto">BAKED TO ORDER & GIFT WRAPPED</p>
                    <p class="description">
                        Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius. Ut eu laoreet ex.
                        Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec
                        lorem erat, finibus in velit placerat, rutrum augue.
                    </p>
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
    flex-wrap: wrap;
    gap: 15px;

    .col-card01 {
        background-image: url(/img/bakery-process-1.jpg);
        background-position: left center;
        background-repeat: no-repeat;
        background-size: cover;
        display: flex;
        flex-wrap: wrap;
        justify-content: right;
        padding: 50px;
        min-height: 800px;

        .title {
            flex-basis: 45%;
        }
    }

    .col-card02 {
        flex-basis: 49%;
        background-image: url(/img/bakery-process-2.jpg);
        background-position: right center;
        background-repeat: no-repeat;
        background-size: cover;
        display: flex;
        flex-wrap: wrap;
        justify-content: left;
        padding: 50px;
        min-height: 800px;

        .title {
            flex-basis: 60%;
        }

    }

    .col-card03 {
        flex-basis: 50%;
        background-color: #F4EFF3;
        padding: 50px;
        min-height: 800px;

        .motto {
            color: #878589;
            font-size: 12px;
            line-height: 1.5;
            font-family: 'Roboto', sans-serif;
            font-weight: 300;
        }

        .title {
            flex-basis: 50%;
            color: #5b2ca2;
            font-size: 60px;
            margin-top: 15px;
            margin-bottom: 15px;
        }
    }

    .col-card04 {
        background-image: url(/img/bakery-process-3.jpg);
        background-position: center center;
        background-repeat: no-repeat;
        background-size: cover;
        display: flex;
        flex-wrap: wrap;
        justify-content: left;
        padding: 50px;
        min-height: 800px;

        .title {
            flex-basis: 45%;
        }
    }

    .title_card {
        display: flex;
        flex-basis: 100%;

        .title {
            color: #ffffff;
            font-size: 56px;
            margin-top: 15px;
        }

        .number {
            color: #ffffff;
            flex-grow: 1;
            font-size: 6em;
            font-family: 'Work Sans', sans-serif;
            font-weight: 200;
            text-align: right;
        }
    }

    .info_card {
        flex-basis: 39%;
        display: flex;
        flex-direction: column;
        margin-top: 250px;

        .motto {
            color: #878589;
            font-size: 12px;
            line-height: 1.5;
            font-family: 'Roboto', sans-serif;
            font-weight: 300;
        }

        .description {
            color: #ffffff;
            font-size: 18px;
            line-height: 30px;
            margin-bottom: 30px;
            margin-top: 15px;
        }
    }
}
</style>
