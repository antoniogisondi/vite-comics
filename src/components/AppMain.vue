<script>
export default {
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
            ]
        }
    },
}
</script>

<template lang="">
    <main>
        <div class="container">
            <div class="row">
                <div class="col">
                    <img src="../assets/img/jumbotron.jpg" alt="">
                </div>
                <div class="col bg-blue">
                    <ul class="nav">
                        <li class="nav-item" v-for="(item, index) in list" :key="index">
                            <img :src="item.img">
                            <a class="nav-link" href="#">{{ item.text }}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
.row {
    font-family: 'Roboto Condensed', sans-serif;

    .col {
        display: flex;
        justify-content: center;

        img {
            width: 100%;
        }
    }

    .bg-blue {
        display: flex;
        justify-content: center;
        background-color: rgba(2, 130, 249, 255);
        width: 100%;

        .nav {
            list-style-type: none;
            display: flex;
            flex-direction: row;

            .nav-item {
                display: flex;
                flex-direction: row;
                align-items: center;
                padding: 35px;

                img {
                    width: 50px;
                    align-self: center;
                }

            }

            .nav-link {
                color: white;
                font-size: 15px;
                text-decoration: none;
                margin-left: 15px;

            }
        }
    }
}
</style>