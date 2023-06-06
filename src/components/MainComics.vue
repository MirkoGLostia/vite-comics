<script>
export default {
    name: "MainComics"
}
</script>

<template>
    <main>
        <section id="content">
            <div class="container">
                CARDS
            </div>
        </section>

        <section id="shop">
            <div class="container">
                <div class="iconShop">
                    <div class="image">
                        <img src="./../assets/img/buy-comics-digital-comics.png" alt="comics">
                    </div>
                    <div class="text">
                        DIGITAL COMICS
                    </div>
                </div>

                <div class="iconShop">
                    <div class="image">
                        <img src="./../assets/img/buy-comics-merchandise.png" alt="merchandise">
                    </div>
                    <div class="text">
                        DC MERCHANDISE
                    </div>
                </div>

                <div class="iconShop">
                    <div class="image">
                        <img src="./../assets/img/buy-comics-subscriptions.png" alt="subs">
                    </div>
                    <div class="text">
                        SUBSCRIPTION
                    </div>
                </div>

                <div class="iconShop">
                    <div class="image">
                        <img src="./../assets/img/buy-comics-shop-locator.png" alt="location">
                    </div>
                    <div class="text">
                        COMIC SHOP LOCATOR
                    </div>
                </div>

                <div class="iconShop">
                    <div class="image">
                        <img src="./../assets/img/buy-dc-power-visa.svg" alt="pay">
                    </div>
                    <div class="text">
                        DC POWER VISA
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>

<style lang="scss" scoped>
@use './../styles/partials/variables' as v;
@use './../styles/partials/mixins.scss' as *;

#content {
    height: 100px;
    background-color: black;
    color: white;
}

#shop {
    height: 120px;
    background-color: v.$myBlue;

    .container {
        @include myFlex;
        @include myFlexPosition;

        .iconShop {
            @include myFlex;
            @include myFlexPosition;

            .image {
                width: 40px;
            }

            .text {
                color: white;
                margin-inline: 8px;
            }
        }
    }
}
</style>
