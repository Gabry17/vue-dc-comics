<template>
    <div class="item">
        <img :src="productObj.thumb" alt="">
        <h3>{{ productObj.series }}</h3>
    </div>
</template>

<script>
export default {
    name: 'AppProps',
    props: {
        productObj: Object,
    }
}
</script>

<style lang="scss" scoped>
    .item{
        margin: 5px;
        width: calc(100% / 6 - 10px);
        padding-bottom: 2em;
        img{
            height: auto;
            width: 100%;
        }
    }
</style>
