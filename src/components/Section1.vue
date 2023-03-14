<script>
</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col-description">
                <ul>
                    <li class="motto">OUR PRODUCTS</li>
                    <li class="title">
                        <h2>All our delectable pastries are backed fresh in our Kitchen very morning, and are made with
                            all-natural, all organic ingredients.</h2>
                    </li>
                    <li class="button">Buy Avada Today!</li>
                </ul>
            </div>
            <div class="col-img">
                <img src="/img/choco-chip-cookies-500x638.jpg" alt="ok">
            </div>
            <div class="col-img">
                <img src="/img/strawberry-jam-cookies-500x638.jpg" alt="ok">
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
            font-size: 25px;
            margin-top: 15px;
            margin-bottom: 40px;
        }

        .button {
            width: 40%;
            padding: 10px 10px 10px 10px;
            color: #ffffff;
            font-size: 18px;
            background-color: #5b2ca2;
            text-align: center;
            border-radius: 6px;
        }
    }

}
</style>
