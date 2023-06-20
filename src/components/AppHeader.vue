<script>
export default {
    data() {
        return {
            navbar_item: [

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
                    <ul class="nav">
                        <li class="nav-item">
                            <a class="nav-link active" href="#">CHARACTERS</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">COMICS</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">MOVIES</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">TV</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">GAMES</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">COLLECTIBLE</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">VIDEOS</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">FANS</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">NEWS</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">SHOP</a>
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
}

.row {
    display: flex;
    flex-direction: row;
}

ul {
    justify-content: flex-end;
    align-items: center;
    list-style-type: none;

    li {
        display: inline-block;
        margin: 20px;
    }
}
</style>