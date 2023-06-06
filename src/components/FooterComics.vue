<script>
export default {
    name: "FooterComics"
}
</script>

<template>
    <footer>
        <nav>
            <div class="container">
                <div class="footNav">
                    <div>
                        <ul>
                            <li class="title">DC COMICS</li>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>

                        <ul>
                            <li class="title">SHOP</li>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>

                    <ul>
                        <li class="title">DC</li>
                        <li>Terms Of Use</li>
                        <li>Privacy policy</li>
                        <li>Ad Choices</li>
                        <li>Adversing</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Rating</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>

                    <ul>
                        <li class="title">SITES</li>
                        <li>DC</li>
                        <li>MAD Magazines</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
                <div class="logo-footer">
                    <img src="./../assets/img/dc-logo-bg.png" alt="logo">
                </div>
            </div>
        </nav>

        <section id="contatti">
            <div class="container">
                <button>
                    SIGN-UP NOW
                </button>

                <div class="follow">
                    <div class="text">
                        FOLLOW US
                    </div>
                    <div class="icon">
                        <div class="image">
                            <img src="./../assets/img/footer-facebook.png" alt="facebook">
                        </div>

                        <div class="image">
                            <img src="./../assets/img/footer-twitter.png" alt="twitter">
                        </div>

                        <div class="image">
                            <img src="./../assets/img/footer-youtube.png" alt="youtube">
                        </div>

                        <div class="image">
                            <img src="./../assets/img/footer-pinterest.png" alt="pinterest">
                        </div>

                        <div class="image">
                            <img src="./../assets/img/footer-periscope.png" alt="periscope">
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
@use './../styles/partials/variables' as v;
@use './../styles/partials/mixins.scss' as *;

nav {
    height: 270px;
    background-image: url(./../assets/img/footer-bg.jpg);

    .container {
        @include myFlex;

        .footNav {
            width: 40%;
            display: flex;
            padding-top: 10px;

            ul {
                color: white;
                margin-inline: 15px;

                .title {
                    font-size: 14px;
                    font-weight: 600;
                    margin-block: 8px;
                    color: white;
                }

                li {
                    font-size: 12px;
                    margin-block: 5px;
                    font-weight: 300;
                    color: rgb(100, 99, 119);
                }
            }
        }

        .logo-footer {
            position: relative;
            top: -40px;
            width: 350px;
        }
    }
}

#contatti {
    height: 90px;
    background-color: v.$myBlack;
    position: relative;
    z-index: 10;

    .container {
        @include myFlex;
        @include myFlexPosition;

        button {
            background-color: v.$myBlack;
            border: 2px solid v.$myBlue;
            padding: 10px;
            color: white;
        }

        .follow {
            display: flex;
            align-items: center;

            .text {
                color: v.$myBlue;
                margin-right: 10px;
                font-weight: 600;
            }

            .icon {
                display: flex;

                .image {
                    width: 25px;
                    margin-inline: 5px;
                }
            }
        }
    }
}
</style>
