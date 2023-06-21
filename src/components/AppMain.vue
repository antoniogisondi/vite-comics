<script>
import AppComicBook from './AppComicBook.vue';
export default {
    components: {
        AppComicBook
    },
    data() {
        return {
            list: [
                {
                    img: './src/assets/img/buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS'
                },
                {
                    img: './src/assets/img/buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE'
                },
                {
                    img: './src/assets/img/buy-comics-subscriptions.png',
                    text: 'SUBSCRIPTION'
                },
                {
                    img: './src/assets/img/buy-comics-shop-locator.png',
                    text: 'COMIC SHOP LOCATOR'
                },
                {
                    img: './src/assets/img/buy-dc-power-visa.svg',
                    text: 'DC POWER VISA'
                }
            ],

            comic_book: [
                {
                    thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    price: "$19.99",
                    series: "ACTION COMICS",
                    type: 'Comic Book'
                },
                {
                    thumb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    price: "$3.99",
                    series: "AMERICAN VAMPIRE 1976",
                    type: 'Comic Book'
                },
                {
                    thumb: "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    price: "$16.99",
                    series: "AQUAMAN",
                    type: 'Graphic Novel'
                },
                {
                    thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    price: "$2.99",
                    series: "BATGIRL",
                    type: 'Comic Book'
                },
                {
                    thumb: "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    price: "$3.99",
                    series: "BATMAN",
                    type: 'Comic Book'
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    price: "$2.99",
                    series: "BATMAN BEYOND",
                    type: 'Comic Book'
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    price: "$3.99",
                    series: "BATMAN/SUPERMAN",
                    type: 'Comic Book'
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    price: "$4.99",
                    series: 'BATMAN/SUPERMAN ANNUAL',
                    type: 'Comic Book'
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    price: "$5.99",
                    series: "BATMAN: THE JOKER WAR ZONE",
                    type: 'Comic Book'
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    price: "$6.99",
                    series: "BATMAN: THREE JOKERS",
                    type: 'Comic Book'
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    price: "$4.99",
                    series: "Batman: White Knight ",
                    type: 'Comic Book'
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    price: "$16.99",
                    series: "CATWOMAN",
                    type: 'Graphic Novel'
                }
            ]
        }
    },
}
</script>

<template lang="">
    <main>
        <div class="container-fluid">
            <div class="row d-flex flex-column">
                <div class="col bg-image">
                    <img src="../assets/img/jumbotron.jpg" alt="">
                </div>

                <div class="col bg-color">
                    <div class="d-flex flex-row flex-wrap width mt-5">
                        <AppComicBook v-for="(item, index) in comic_book" :key="index"
                            :img="item.thumb"
                            :series="item.series"
                            :type="item.type"
                            :price="item.price"
                        />
                    </div>

                    <div class="button d-flex justify-content-center pb-3 pt-5">
                        <button>LOAD MORE</button>
                    </div>

                    <div class="badge">
                        <span>CURRENT SERIES</span>
                    </div>
                </div>

                <div class="col bg-blue d-flex justify-content-center">
                    <ul class="nav d-flex flex-row p-2">
                        <li class="nav-item d-flex flex-row align-items-center m-4" v-for="(item, index) in list" :key="index">
                            <img :src="item.img">
                            <a class="nav-link text" href="#">{{ item.text }}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
.bg-image {
    img {
        width: 100%;
    }
}

.bg-blue {
    background-color: rgba(2, 130, 249, 255);
    width: 100%;

    .nav {
        list-style-type: none;

        img {
            width: 40px;
        }

    }

    .text {
        color: white;
        font-size: 15px;
        text-decoration: none;

    }
}

.bg-color {
    position: relative;
    background-color: rgba(28, 28, 28, 255);

    .width {
        width: calc(100% / 1.3);
        margin: 0 auto;
    }

    .button {
        button {
            color: white;
            background-color: rgba(2, 130, 249, 255);
            border: none;
            padding: 5px 60px;
        }
    }

    .badge {
        left: 12.5%;
        top: -2%;
        position: absolute;

        span {
            color: white;
            font-size: 20px;
            background-color: rgba(2, 130, 249, 255);
            border: none;
            padding: 10px 25px;
        }
    }
}
</style>