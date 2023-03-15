<script>
import BannerFooter from './BannerFooter.vue'

export default {
    data() {
        return {
            linksFooter: [
                {
                    link: 'SHOP',
                },
                {
                    link: 'ABOUT',
                },
                {
                    link: 'GALLERY',
                },
                {
                    link: 'LOCATIONS',
                },
                {
                    link: 'JOURNAL',
                },
                {
                    link: 'CONTACT',
                },
                {
                    link: 'ORDERS',
                },
            ]
        }
    },
    components: {
        BannerFooter,
    },
}

</script>

<template>
    <BannerFooter></BannerFooter>
    <footer>
        <div class="row">
            <div class="col-menu">
                <div class="col-logo">
                    <img src="/img/avada-bakery-logo-retina.png" alt="ok">
                </div>
                <div class="col_nav_menu">
                    <ul>
                        <li v-for="el in linksFooter">
                            <a href="#">{{ el.link }}</a>
                        </li>
                        <li>
                            <font-awesome-icon icon="fa-solid fa-cart-shopping" class="icon" />
                            <span>0</span>
                        </li>
                    </ul>
                </div>
                <div class="col-copyright">
                    <font-awesome-icon icon="fa-regular fa-copyright" class="icon" />
                    <span>Copyright 2019 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by WordPress</span>
                </div>
            </div>

            <div class="col-social">
                <div class="col-title">
                    <h3>Subscribe to our Newsletter</h3>
                </div>
                <div class="col-call-to-action">
                    <input class="text-area" type="text" placeholder="Enter Email address*">
                    <span class="button">
                        Subscribe
                    </span>
                </div>
                <div class="col_icon_social">
                    <font-awesome-icon icon="fa-brands fa-instagram" />
                    <font-awesome-icon icon="fa-brands fa-twitter" />
                    <font-awesome-icon icon="fa-brands fa-facebook" />
                    <font-awesome-icon icon="fa-brands fa-pinterest-p" />
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../src/style/general.scss' as *;

footer {
    padding: 90px;
}

.row {
    display: flex;
    align-items: center;

    .col-social,
    .col-menu {
        flex-basis: 50%;
        display: flex;
        flex-direction: column;
    }

    .col-menu {
        .col-logo {

            img {
                width: 160px;
                padding: 1.25rem 0rem;
                padding-left: 2.18rem;
            }
        }

        .col_nav_menu {
            margin-top: 45px;
            margin-bottom: 130px;

            ul {
                display: flex;
                align-items: center;
                gap: 2.37rem;
                color: #5b2ca2;

                li {
                    padding: 0.4rem;
                    font-size: 0.75rem;
                }
            }

            span {
                color: #5b2ca2;
                padding: 3px;
                background-color: #F0EDF5;
                display: inline-block;
                width: 20px;
                height: 20px;
                border-radius: 50%;
                text-align: center;
                font-size: 0.75rem;
            }

            .icon {
                margin-right: 5px;
                font-size: 0.75rem;
            }

        }

        .col-copyright {
            color: #878589;
            font-size: 15px;
            font-family: 'Source Serif Pro', serif;
            font-weight: 400;
            margin-bottom: 20px;

            .icon {
                margin-right: 5px;
                font-size: 10px;
            }
        }
    }

    .col-social {
        text-align: right;

        .col-title {
            color: #5b2ca2;
            font-size: 25px;
            margin-top: 10px;
            margin-bottom: 50px;
        }

        .col-call-to-action {
            margin-top: 45px;
            margin-bottom: 130px;
            font-family: 'Roboto', sans-serif;
            font-weight: 300;

            .text-area {
                width: 50%;
                margin-right: 10px;
                padding: 10px 15px 10px 15px;
                color: #ffffff;
                font-size: 14px;
                text-align: left;
                border-radius: 6px;
                border: 1px solid #878589;
            }

            .button {
                width: 15%;
                padding: 10px 15px 10px 15px;
                color: #ffffff;
                font-size: 15px;
                background-color: #5b2ca2;
                text-align: center;
                border-radius: 6px;
                font-family: 'Roboto', sans-serif;
                font-weight: 300;
            }

        }

        .col_icon_social {
            display: flex;
            align-self: self-end;
            gap: 30px;
            color: #5b2ca2;
            font-size: 18px;
            margin-bottom: 20px;
        }
    }
}
</style>
