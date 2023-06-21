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
        <div class="container">
            <div class="row">
                <div class="container-col">
                    <div class="col">
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
    
                    <div class="col">
                        <ul>
                            <li>
                                <h3>DC</h3>
                            </li>
                            <li v-for="item in dc_array">{{ item }}</li>
                        </ul>
                    </div>
    
                    <div class="col">
                        <ul>
                            <li>
                                <h3>SITES</h3>
                            </li>
                            <li v-for="item in sites_array">{{ item }}</li>
                        </ul>
                    </div>
                </div>
            </div>
            
            <div class="row-footer">
                <div class="col">
                 <button>SIGN-UP NOW!</button>
                </div>

                <div class="col-2">
                    <h3>FOLLOW US</h3>
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
footer {
    font-family: 'Roboto Condensed', sans-serif;


    .container {
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;

        .row {
            display: flex;
            justify-content: space-between;
            max-width: 1170px;
            background-image: url('../assets/img/dc-logo-bg.png');
            background-size: 500px;
            background-repeat: no-repeat;
            background-position: right;

            .container-col {
                display: flex;

                h3 {
                    color: white;
                    margin: 10px 0;
                    font-size: 20px;
                }

                .col li {
                    list-style-type: none;
                    color: rgba(111, 111, 111, 255);
                    font-size: 15px;
                    padding: 3px 0;
                }
            }
        }
    }


    .row-footer {
        background-color: rgba(48, 48, 48, 255);
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        align-items: center;

        .col button {
            background-color: transparent;
            border-color: rgba(10, 114, 212, 255);
            padding: 10px;
            font-size: 15px;
            font-weight: 700;
            color: white;

        }

        .col-2 {
            display: inline-flex;
            justify-content: center;
            padding: 20px 0 15px;

            h3 {
                color: rgba(2, 130, 249, 255);
                padding: 0 20px 15px;
            }

            img {
                width: 30px;
                height: 30px;
                padding: 15px 5px;
            }

        }
    }
}
</style>