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
        <div class="container-fluid">
            <div class="row">
                <div class="col d-flex justify-content-start m-3">
                    <img src="../assets/img/dc-logo.png" alt="">
                </div>
                <div class="col d-flex justify-content-start">
                    <ul>
                        <li class="m-2 p-0" v-for="(item, index) in navbar_item">
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
    font-weight: 700;
}

ul {
    list-style-type: none;

    li {
        display: inline-block;
        margin: 12px;

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


.col {
    display: flex;
    align-items: center;
    justify-content: center;

    img {
        max-width: 65%;
    }
}
</style>