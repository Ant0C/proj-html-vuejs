<script>
</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col-info">
                <ul>
                    <li class="motto">LOCATIONS</li>
                    <li class="title">
                        <h2>Visit our Bakeries</h2>
                    </li>
                </ul>
            </div>
            <div class="col-location">
                <div class="col-location-nw">
                    <img src="/img/new-york-bk-1200x794.jpg" alt="ok">
                    <h3>New York</h3>
                    <div class="info_location">
                        <div>
                            <p>CALL US </p>
                            <p class="info"> 1.800.458.556</p>
                        </div>
                        <div>
                            <p>OPEN ALL WEEK</p>
                            <p class="info">9:00 AM - 6:00 PM</p>
                        </div>
                        <a href="#" class="button"> View Map</a>
                    </div>
                </div>
                <div class="col-location-lo">
                    <img src="/img/london-bk-1200x794.jpg" alt="ok">
                    <h3>London</h3>
                    <div class="info_location">
                        <div>
                            <p>CALL US </p>
                            <p class="info"> 1.800.458.556</p>
                        </div>
                        <div>
                            <p>OPEN ALL WEEK </p>
                            <p class="info"> 9:00 AM - 6:00 PM</p>
                        </div>
                        <a href="#" class="button">View Map</a>
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
        font-size: 40px;
        margin-top: 15px;
        margin-bottom: 40px;
    }

    .button {
        padding: 10px;
        color: #B1ADAB;
        font-size: 18px;
        background-color: #ffffff;
        text-align: center;
        border-radius: 6px;
        font-family: 'Roboto', sans-serif;
        font-weight: 300;
    }

    .button:hover {
        color: #e9dedc;
        background-color: #5b2ca2;
        transition: all .2s;
    }


    .col-location {
        display: flex;

        h3 {
            color: #5b2ca2;
            font-size: 36px;
            margin: 40px 0px;
        }

        .col-location-nw {
            display: flex;
            flex-direction: column;
            background-color: #F1F9FB;

            .info_location {
                display: flex;
                justify-content: space-around;
                margin-bottom: 25px;

                div {
                    flex-basis: calc(100% *(3/12));

                    p {
                        color: #878589;
                        font-size: 12px;
                    }

                    .info {
                        font-size: 18px;
                        margin-top: 5px;
                    }
                }
            }
        }

        .col-location-lo {
            display: flex;
            flex-direction: column;
            background-color: #FAF3E3;

            .info_location {
                display: flex;
                justify-content: space-around;
                margin-bottom: 25px;

                div {
                    flex-basis: calc(100% *(3/12));

                    p {
                        color: #878589;
                        font-size: 12px;
                    }

                    .info {
                        font-size: 18px;
                        margin-top: 5px;
                    }
                }
            }
        }
    }
}
</style>
