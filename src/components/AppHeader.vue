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
    display: flex;
    justify-content: center;
    align-items: center;
}

.row {
    display: flex;
    flex-direction: row;

    ul {
        justify-content: flex-end;
        align-items: center;
        list-style-type: none;

        li {
            display: inline-block;
            margin: 20px;

            a {
                font-size: 13px;
                text-decoration: none;
                color: rgba(74, 72, 71, 255);
            }
        }
    }

    .col {
        display: flex;
        align-items: center;

        img {
            max-width: 65%;
        }
    }
}
</style>