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
        <div class="container-fluid bg-image">
            <div class="row bg-image-2">
                <div class="container-col d-flex justify-content-center m-4">
                    <div class="col-2">
                        <ul>
                            <li>
                                <h3>DC COMICS</h3>
                            </li>
                            <li v-for="item in dc_comics_array">{{ item }}</li>
                        </ul>
    
                        <ul>
                            <li>
                                <h3>SHOP</h3>
                            </li>
                            <li v-for="item in shop_array">{{ item }}</li>
                        </ul>
                    </div>
    
                    <div class="col-2">
                        <ul>
                            <li>
                                <h3>DC</h3>
                            </li>
                            <li v-for="item in dc_array">{{ item }}</li>
                        </ul>
                    </div>
    
                    <div class="col-2">
                        <ul>
                            <li>
                                <h3>SITES</h3>
                            </li>
                            <li v-for="item in sites_array">{{ item }}</li>
                        </ul>
                    </div>
                </div>
            </div>
            
            <div class="row row-col-3 d-flex flex-row bg-color">
                <div class="col m-5 d-flex justify-content-start">
                 <button>SIGN-UP NOW!</button>
                </div>

                <div class="col d-flex justify-content-end align-items-center">
                    <h3>FOLLOW US</h3>
                    <div class="link">
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
        </div>
    </footer>
</template>

<style lang="scss" scoped>
.bg-image {
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;

    .bg-image-2 {
        max-width: 1170px;
        background-image: url('../assets/img/dc-logo-bg.png');
        background-size: 500px;
        background-repeat: no-repeat;
        background-position: right;
        padding: 40px 0;
        padding-bottom: 60px;

        h3 {
            color: white;
            font-size: 20px;
            margin: 0;
        }

        li {
            list-style-type: none;
            color: rgba(111, 111, 111, 255);
            font-size: 15px;

        }
    }
}



.bg-color {
    background-color: rgba(48, 48, 48, 255);

    .col button {
        background-color: transparent;
        border-color: rgba(10, 114, 212, 255);
        padding: 10px;
        font-size: 15px;
        font-weight: 700;
        color: white;

    }

    h3 {
        color: rgba(2, 130, 249, 255);
        padding: 20px;
    }

    .link {
        a {
            img {
                width: 50px;
                height: 50px;
                padding: 10px;
            }
        }
    }
}
</style>