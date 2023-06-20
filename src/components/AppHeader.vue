<script>
export default {
    data() {
        return {
            navbar_item: ['CHARACTERS', 'COMICS', 'MOVIES', 'TV', 'GAMES', 'COLLECTIBLE', 'VIDEOS', 'FANS', 'NEWS', 'SHOP']
        }
    }
}
</script>

<template lang="">
    <header>
        <div class="container">
            <div class="row">
                <div class="col">
                    <img src="../assets/img/dc-logo.png" alt="">
                </div>
                <div class="col">
                    <ul class="nav">
                        <li class="nav-item" v-for="(item, index) in navbar_item">
                            <a class="nav-link" href="#">{{ item }}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header {
    font-family: 'Roboto Condensed', sans-serif;
    font-weight: 700;
}

.row {
    display: flex;
    flex-direction: row;
    justify-content: space-around;

    .col {
        ul {
            list-style-type: none;

            li {
                display: inline-block;
                margin: 20px;

                a {
                    font-size: 15px;
                    text-decoration: none;
                    color: rgba(74, 72, 71, 255);

                    &:hover {
                        color: rgba(2, 130, 249, 255);
                    }
                }
            }
        }
    }
}

.col {
    display: flex;
    align-items: center;
    justify-content: center;

    img {
        max-width: 65%;
    }
}
</style>