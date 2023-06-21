<script>
export default {
    props: {
        img: String,
        price: String,
        series: String,
        type: String
    }
}
</script>

<template>
    <div class="m-3">
        <img :src="img">
        <h2 class="d-flex flex-wrap">{{ series }}</h2>
        <h3>{{ type }}</h3>
        <h4>{{ price }}</h4>
    </div>
</template>

<style lang="scss" scoped>
img {
    width: 170px;
    height: 200px
}

h2 {
    margin-top: 15px;
    font-size: 13px;
    color: white;
}

h3,
h4 {
    font-size: 13px;
    color: white;
}
</style>