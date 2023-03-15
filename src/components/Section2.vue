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
                <img src="/img/corporate-bg.jpg" alt="ok">
                <img src="/img/wedding-bg.jpg" alt="ok">
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
    }

}
</style>
