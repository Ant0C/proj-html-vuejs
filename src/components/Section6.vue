<script>
</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col-social">
                <div>
                    <img src="/img/social-1.jpg" alt="ok">
                </div>
                <div class="call-to-action">
                    <ul>
                        <li class="motto">
                            <h2>MADE FOR SHARING</h2>
                        </li>
                        <li class="title">
                            Let's stay in touch
                        </li>
                        <li class="button"><font-awesome-icon icon="fa-brands fa-instagram" class="icon" />Follow Us</li>
                    </ul>
                </div>
                <div>
                    <img src="/img/social-2.jpg" alt="ok">
                </div>
            </div>
            <div class="col-social-img">
                <div>
                    <img src="/img/social-3.jpg" alt="ok">
                </div>
                <div>
                    <img src="/img/social-5.jpg" alt="ok">
                </div>
                <div>
                    <img src="/img/social-4.jpg" alt="ok">
                </div>
                <div>
                    <img src="/img/social-6.jpg" alt="ok">
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

    img {
        width: 389px;
    }

    .col-social {
        flex-basis: 100%;
        display: flex;
        gap: 15px;


        .call-to-action {
            flex-basis: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            background-color: #F2EEF4;
            margin: 0px 20px;

            .motto {
                color: #878589;
                font-size: 12px;
                line-height: 1.5;
                font-family: 'Roboto', sans-serif;
                font-weight: 300;
            }

            .title {
                color: #5b2ca2;
                font-family: 'Source Serif Pro', serif;
                font-weight: 700;
                font-size: 36px;
                margin-top: 15px;
                margin-bottom: 40px;
            }

            .button {
                width: 50%;
                margin: 0 auto;
                padding: 15px;
                color: #ffffff;
                font-size: 18px;
                background-color: #5b2ca2;
                text-align: center;
                border-radius: 6px;
                font-family: 'Roboto', sans-serif;

                .icon {
                    margin-right: 5px
                }
            }
        }
    }

    .col-social-img {
        flex-basis: 100%;
        display: flex;
        margin-top: 15px;

        div {
            margin: 0px 15px;
        }

        div :first-child {
            margin-left: -15px;
        }

        div :last-child {
            margin-left: -15px;
        }
    }

}
</style>
