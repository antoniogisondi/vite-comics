<script>
export default {
    data() {
        return {
            dc_comics_array: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News'],
            shop_array: ['Shop DC', 'Shop DC Collectibles'],
            dc_array: ['Terms Of Use', 'Privacy policy (New)', 'Ad Choices', 'Advertising', 'Jobs', 'Subscription', 'Talent Workshop', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us'],
            sites_array: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
        }
    },
}
</script>


<template lang="">
    <footer>
        <div class="container-top">
            <div class="row d-flex">
                <div class="col">
                    <div class="first-col-list">
                        <ul>
                            <h2>DC COMICS</h2>
                            <li v-for="(item,index) in dc_comics_array" :key="index">{{ item }}</li>
                        </ul>

                        <ul id="sublist">
                            <h2>SHOP</h2>
                            <li v-for="(item,index) in shop_array" :key="index">{{ item }}</li>
                        </ul>
                    </div>

                    <div class="second-col-list">
                        <ul>
                            <h2>DC </h2>
                            <li v-for="(item,index) in dc_array" :key="index">{{ item }}</li>
                        </ul>
                    </div>

                    <div class="third-col-list">
                        <ul>
                            <h2>SITES</h2>
                            <li v-for="(item,index) in sites_array" :key="index">{{ item }}</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="container-bottom">
            <div class="row d-flex">
                <div class="col-button d-flex">
                    <button>SIGN-UP NOW</button>

                </div>
                <div class="col-image d-flex justify-content-end">
                    <h3>FOLLOW US</h3>
                    <!-- icone social -->
                    <a href="#">
                        <img src="../assets/img/footer-facebook.png" alt="">
                    </a>
                    <a href="#">
                        <img src="../assets/img/footer-periscope.png" alt="">
                    </a>
                    <a href="#">
                        <img src="../assets/img/footer-pinterest.png" alt="">
                    </a>
                    <a href="#">
                        <img src="../assets/img/footer-twitter.png" alt="">
                    </a>
                    <a href="#">
                        <img src="../assets/img/footer-youtube.png" alt="">
                    </a>
                </div>

            </div>
        </div>

    </footer>
</template>


<style lang="scss" scoped>
.container-top {
    background-image: url('../assets/img/footer-bg.jpg');



    .row {
        max-width: 1170px;
        margin: 0 auto;
        background-image: url('../assets/img/dc-logo-bg.png');
        background-size: 500px;
        background-repeat: no-repeat;
        background-position: right;
        padding: 40px 0;
        padding-bottom: 60px;



        .col {
            display: flex;

            ul {
                list-style-type: none;
                padding-right: 40px;
                color: rgba(243, 243, 243, 0.531);

                li {
                    &:hover {
                        color: white;
                    }
                }

                h2 {
                    padding-bottom: 10px;
                    color: white;
                }
            }

            #sublist {
                padding-top: 10px;
            }
        }
    }


}

.container-bottom {
    background-color: rgb(62, 62, 62);
    padding: 20px 0;


    .row {
        max-width: 1170px;
        margin: 0 auto;


        .col-button {
            width: 50%;

            button {
                background-color: transparent;
                padding: 15px;
                border-color: rgb(5, 136, 237);
                color: white;
                font-weight: 800;
            }

        }

        .col-image {
            width: 50%;

            h3 {
                color: rgb(38, 143, 234);
                padding-top: 10px;
                padding-right: 40px;
            }

            img {
                margin-right: 10px;
                height: 30px;
                margin-top: 5px;

            }
        }

    }
}
</style>