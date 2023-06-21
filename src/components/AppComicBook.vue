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
    <div class="m-4">
        <img :src="img">
        <h2>{{ series }}</h2>
        <h3>{{ type }}</h3>
        <h4>{{ price }}</h4>
    </div>
</template>

<style lang="scss" scoped>
img {
    width: 170px;
    height: 200px
}

h2,
h3,
h4 {
    font-size: 15px;
}
</style>