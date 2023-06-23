<script>
export default {
    data() {
        return {
            navbar_item: [
                {
                    text: 'CHARACTERS',
                    active: false
                },
                {
                    text: 'COMICS',
                    active: false
                },
                {
                    text: 'MOVIES',
                    active: false
                },
                {
                    text: 'TV',
                    active: false
                },
                {
                    text: 'GAMES',
                    active: false
                },
                {
                    text: 'COLLECTIBLE',
                    active: false
                },
                {
                    text: 'VIDEOS',
                    active: false
                },
                {
                    text: 'FANS',
                    active: false
                },
                {
                    text: 'NEWS',
                    active: false
                },
                {
                    text: 'SHOP',
                    active: false
                }
            ]
        }
    }
}
</script>

<template lang="">
    <header>
        <div class="container-fluid">
            <div class="row d-flex flex-row m-3">
                <div class="col-2 d-flex justify-content-center">
                    <img src="../assets/img/dc-logo.png" alt="">
                </div>
                <div class="col-10 d-flex justify-content-end align-items-center">
                    <ul>
                        <li class="m-4 active" v-for="(item, index) in navbar_item" :class="item.active ? 'active' : '' " :key="index">
                            <a href="#">{{ item.text }}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
.active:hover {
    border-bottom: 4px solid rgba(2, 130, 249, 255);

}

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

img {
    width: 35%;
}
</style>