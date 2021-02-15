<template>
    <div class="header">
        <div class="header__container">
            <ul class="header__top">
                <li class="header__logo header__icon"><a href="#">MoGo</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Service</a></li>
                <li><a href="#">Work</a></li>
                <li><a href="#">Blog</a></li>
                <li><a href="#">Contact</a></li>
                <li class="header__icon">
                    <a class="header__icon-cart" href="#"></a>
                </li>
                <li class="header__icon">
                    <a class="header__icon-search" href="#"></a>
                </li>
            </ul>
            <div class="header__center">
                <p class="header__title">Creative Template</p>
                <p class="header__subtitle">Welcome<br />to MoGo</p>
                <div class="header__line"></div>
                <button>Learn more</button>
            </div>
            <ul class="header__bottom">
                <li><a href="#">01<span>Intro</span></a></li>
                <li><a href="#">02<span>Work</span></a></li>
                <li><a href="#">03<span>About</span></a></li>
                <li><a href="#">04<span>Contacts</span></a></li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>

    .header {
        background: url("./eagle1.png") center center no-repeat;
        height: 100vh;
        position: relative;

        &::before {
            display: block;
            content: "";
            background: linear-gradient(#f38181 0%, #fce38a 100%);
            position: absolute;
            width: 100%;
            height: 100%;
            opacity: 0.9;

        }

        &__container {
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            height: 100%;
            width: 1200px;
            margin: 0 auto;
            position: relative;
        }

        &__top {
            margin: 0;
            display: flex;
            justify-content: flex-end;
            padding: 20px 0 0;
            align-items: center;

            li {
                list-style: none;
                margin-left: 50px;

                &:first-child {
                    margin-left: 0;
                }

                a {
                    color: #ffffff;
                    text-decoration: none;
                    display: block;
                    font-size: 14px;
                    position: relative;
                    text-transform: uppercase;
                    transition: all 0.2s ease-in;

                    &::after {
                        display: block;
                        content: '';
                        position: absolute;
                        border-bottom: 3px solid #fce38a;
                        width: 100%;
                        margin-top: 10px;
                        opacity: 0;
                        transition: opacity 0.2s ease-in;
                    }

                    &:hover {
                        color: #fce38a;

                        &::after {
                            opacity: 1;
                        }
                    }
                }
            }
        }

        &__icon {

            &-cart {
                background: #fff;
                display: block;
                width: 18px;
                height: 18px;
                -webkit-mask: url("./cart.png") center center no-repeat;
                mask: url("./cart.png") center center no-repeat;

                &:hover {
                    background: #fce38a;
                }
            }

            &-search {
                background:  #fff;
                display: block;
                width: 18px;
                height: 18px;
                -webkit-mask: url("./search.png") center center no-repeat;
                mask: url("./search.png") center center no-repeat;

                &:hover {
                    background: #fce38a;

                }
            }

            a {

                &:hover {

                    &::after {
                        border-bottom: none !important;
                    }
                }
            }
        }

        &__logo {
            color: #ffffff;
            font-weight: bold;
            margin-right: auto;

            a {
                font-size: 30px !important;
                text-transform: initial !important;
            }
        }

        &__center {
            display: flex;
            flex-direction: column;
            align-items: center;

            button {
                padding: 0 30px;
                height: 40px;
                font-size: 14px;
                font-weight: 700;
                color:#ffffff;
                border: 3px solid #ffffff;
                background: none;
                outline: none;
                text-transform: uppercase;
                cursor: pointer;
                transition: all 0.2s ease-in;

                &:hover {
                    color: #fce38a;
                    border: 3px solid #fce38a;
                }
            }
        }

        &__title {
            font-family: "kaushan Script", sans-serif;
            font-size: 72px;
            color: #ffffff;
            margin-bottom: 42px;
            margin-top: 0;
            line-height: 1em;
        }

        &__subtitle {
            font-size: 150px;
            color: #ffffff;
            font-weight: 700;
            margin: 0;
            text-align: center;
            line-height: 140px;
            text-transform: uppercase;
        }

        &__line {
            width: 60px;
            height: 3px;
            background-color: #ffffff;
            margin: 55px 0 50px;
        }

        &__bottom {
            display: flex;
            margin: 0;
            padding: 0;

            li {
                list-style: none;
                flex-grow: 1;
                margin: 0 30px 24px 0;
                font-size: 24px;
                font-weight: 700;
                color: #ffffff;

                &:last-child {
                    margin-right: 0;
                }

                a {
                    text-decoration: none;
                    color: rgba(255, 255, 255, 0.7);
                    position: relative;
                    display: block;
                    width: 100%;
                    height: 100%;
                    border-top: 3px solid rgba(255, 255, 255, 0.5);
                    padding-top: 11px;
                    transition: all 0.2s ease-in;

                    &::before {
                        display: block;
                        content: "";
                        width: 0px;
                        height: 3px;
                        background: #f38181;
                        position: absolute;
                        top: -3px;
                        transition: width 0.2s ease-in;
                    }

                    &:hover {
                        color: #ffffff;
                        border-top: 3px solid rgba(255, 255, 255, 1);

                        &::before {
                            width: 70px;
                        }
                    }
                }
            }

            span {
                font-size: 18px;
                text-transform: uppercase;
                margin-left: 10px;
                color: #ffffff;
                font-weight: 400;
            }
        }
    }
</style>
