<script>
export default {

}
</script>

<template lang="">
    <main>
        <div class="container">
            <div class="row">
                <div class="col bg-black">
                    <h1> --Content goes here-- </h1>
                </div>
                <div class="col bg-blue">
                    <ul class="nav">
                        <li class="nav-item-big">
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                            <a class="nav-link" href="#">DIGITAL COMICS</a>
                        </li>
                        <li class="nav-item">
                            <img src="../assets/img/buy-comics-merchandise.png" alt="">
                            <a class="nav-link" href="#">COMICS</a>
                        </li>
                        <li class="nav-item">
                            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                            <a class="nav-link" href="#">MOVIES</a>
                        </li>
                        <li class="nav-item">
                            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                            <a class="nav-link" href="#">TV</a>
                        </li>
                        <li class="nav-item-svg">
                            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                            <a class="nav-link" href="#">GAMES</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
.row {

    .bg-black {
        background-color: black;

        h1 {
            color: white;
        }
    }

    .bg-blue {
        display: flex;
        justify-content: center;
        background-color: rgba(2, 130, 249, 255);
        padding: 50px;

        .nav {
            list-style-type: none;
            display: flex;
            flex-direction: row;

            .nav-item img {
                max-width: 30%;
            }

            .nav-item-big img {
                max-width: 20%;
            }
        }
    }
}
</style>