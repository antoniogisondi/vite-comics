<script>
export default {
    data() {
        return {
            navbar_item: [
                {
                    text: 'CHARACTERS',
                    active: true
                },
                {
                    text: 'COMICS',
                    active: true
                },
                {
                    text: 'MOVIES',
                    active: true
                },
                {
                    text: 'TV',
                    active: true
                },
                {
                    text: 'GAMES',
                    active: true
                },
                {
                    text: 'COLLECTIBLE',
                    active: true
                },
                {
                    text: 'VIDEOS',
                    active: true
                },
                {
                    text: 'FANS',
                    active: true
                },
                {
                    text: 'NEWS',
                    active: true
                },
                {
                    text: 'SHOP',
                    active: true
                }
            ]
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
                    <ul>
                        <li v-for="(item, index) in navbar_item">
                            <a href="#">{{ item.text }}</a>
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