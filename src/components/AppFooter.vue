<script>
export default {

}
</script>

<template lang="">
    <footer>
        <div class="container">
            <div class="row bg-image">
                <div class="col">
                    <ul>
                        <li>
                            <h3>DC COMICS</h3>
                        </li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                    </ul>

                    <ul>
                        <li>
                            <h3>SHOP</h3>
                        </li>
                        <li>Characters</li>
                        <li>Characters</li>
                    </ul>
                </div>

                <div class="col">
                    <ul>
                        <li>
                            <h3>DC</h3>
                        </li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                    </ul>
                </div>

                <div class="col">
                    <ul>
                        <li>
                            <h3>SITES</h3>
                        </li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                    </ul>
                </div>
            </div>
            
            <div class="row footer">
                <div class="col">
                 <button>SIGN-UP NOW!</button>
                </div>

                <div class="col-2">
                 <h2>FOLLOW US</h2>
                 <img src="../assets/img/footer-facebook.png" alt="">
                 <img src="../assets/img/footer-periscope.png" alt="">
                 <img src="../assets/img/footer-pinterest.png" alt="">
                 <img src="../assets/img/footer-twitter.png" alt="">
                 <img src="../assets/img/footer-youtube.png" alt="">
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
footer {
    .bg-image {
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        display: flex;
        flex-direction: row;

        .col ul {
            list-style-type: none;
        }
    }

    .footer {
        background-color: rgba(48, 48, 48, 255);
        display: flex;
        flex-direction: row;
        justify-content: space-between;

        .col-2 {
            display: inline-flex;

        }
    }
}
</style>