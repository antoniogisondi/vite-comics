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
    <div>
        <img :src="img">
        <h2>{{ series }}</h2>
        <h3>{{ type }}</h3>
        <h4>{{ price }}</h4>
    </div>
</template>

<style lang="">
    
</style>