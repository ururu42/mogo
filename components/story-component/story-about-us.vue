<template>
    <div class='story'>
        <div class='story__container'>
            <p class='story__title'>What we do</p>
            <p class='story__subtitle'>Story about us</p>
            <p class='story__text'>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
            <ul class='story__foto'>
                <li>
                    <a href='#'>
                        <img src="./story1.jpg" />
                        <span>
                            <img src="./story-icon.png" />Super team
                        </span>
                    </a>
                </li>
                <li>
                    <a href='#'>
                        <img src="./story2.jpg" />
                        <span>
                            <img src="./story-icon.png" />Super team
                        </span>
                    </a>
                </li>
                <li>
                    <a href='#'>
                        <img src="./story3.jpg" />
                        <span>
                            <img src="./story-icon.png" />Super team
                        </span>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>

    .story {
        background: #fff;
        padding: 86px 0 88px;

        &__container {
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            width: 1200px;
            margin: 0 auto;
            align-items: center;
        }

        &__title {
            margin: 0 0 10px;
            font-family: "Kaushan Script", sans-serif;
            font-size: 24px;
            font-weight: 400;
            color: #333333;
        }

        &__subtitle {
            font-family: "Montserrat", sans-serif;
            font-size: 30px;
            font-weight: 700;
            text-transform: uppercase;
            color: #333333;
            margin: 0;

            &::after {
                display: block;
                content: '';
                position: relative;
                border-bottom: 3px solid #f38181;
                width: 60px;
                margin: 30px auto 27px;
            }
        }

        &__text {
            font-family: "Roboto", sans-serif;
            font-size: 15px;
            font-weight: 400;
            text-align: center;
            color: #999999;
            margin-bottom: 99px;
            line-height: 24px;
            display: block;
            max-width: 960px;
        }

        &__foto {
            display: flex;
            justify-content: space-between;
            margin: 0;
            padding: 0;
            width: 100%;

            li {
                list-style: none;
                background: #95e1d3;

                a {
                    position: relative;
                    display: flex;
                    transition: transform 0.2s ease-in;

                    & > img {

                    }

                    span {
                        display: flex;
                        justify-content: center;
                        align-items: center;
                        flex-direction: column;
                        background: linear-gradient(rgba(243, 129, 129, 0.9) 0%, rgba(252, 227, 138, 0.9) 100%);
                        position: absolute;
                        top: 0;
                        left: 0;
                        width: 100%;
                        height: 100%;
                        font-size: 18px;
                        font-weight: 700;
                        text-transform: uppercase;
                        color: #fff;
                        opacity: 0;
                        transition: opacity 0.2s ease-in;

                        img {
                            margin-bottom: 6px;

                        }
                    }

                    &:hover {
                        transform: translate(-12px, -12px);

                        span {
                            opacity: 1;
                        }
                    }
                }
            }
        }
    }
</style>
