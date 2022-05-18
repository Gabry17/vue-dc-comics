<template>
    <div class="header">
        <img src="../assets/img/dc-logo.png" alt="logo">
        <ul>
            <li v-for="(item, index) in links" :key="index">
            <a :class="{'active': item.active}" href="">{{item.title}}</a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'AppHeader',
    data: function(){
        return{
            links:[
                {
                    title: 'characters',
                    active: false
                },
                {
                    title: 'comics',
                    active: true
                },
                {
                    title: 'movies',
                    active: false
                },
                {
                    title: 'tv',
                    active: false
                },
                {
                    title: 'games',
                    active: false
                },
                {
                    title: 'collectibles',
                    active: false
                },
                {
                    title: 'videos',
                    active: false
                },
                {
                    title: 'fans',
                    active: false
                },
                {
                    title: 'news',
                    active: false
                },
                {
                    title: 'shop',
                    active: false
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
$color-primary-color: #0080ff;
.header{
    height: 100px;
    display: flex;
    width: 70%;
    margin: 0 auto;
    justify-content: space-between;
    align-items: center;
    img{
        height: 50px;
        vertical-align: middle;
    }
    ul{
        display: flex;
        line-height: 100px;
        li{
            margin: .5rem;
        }   
        a{
            color: black;
            text-transform: uppercase;
        }
    }
    .active{
        color: $color-primary-color;
        padding: 2.4em 0;
        border-bottom: 2px solid $color-primary-color;
    }
}
</style>