<script>
import shopCard from './shopCard.vue';

export default {
    name: "MainComics",
    components: {
        shopCard
    },
    data() {
        return {
            comics: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    }
}
</script>

<template>
    <main>
        <section id="content">
            <div class="container">
                <div class="comic-shop">
                    <shopCard v-for="comic in comics" :details="comic" />
                </div>
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
    background-color: black;
    color: white;
    height: fit-content;

    .container {
        padding: 10px;
        width: 100%;

        .comic-shop {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 20px;
            overflow: hidden;
            overflow-y: auto;
        }

    }

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
