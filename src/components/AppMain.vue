<template>
<div class="main">
    <div class="main-top">
        <div class="cont-top">
            <span>Content goes here</span>
        </div>
    </div>
    <div class="main-bottom">
        <div class="cont-bottom">
            <ul>
                <li><img src="../assets/img/buy-comics-digital-comics.png" alt=""><a href="">digital comics</a></li>
                <li><img src="../assets/img/buy-comics-merchandise.png" alt=""><a href="">dc merchandise</a></li>
                <li><img src="../assets/img/buy-comics-subscriptions.png" alt=""><a href="">subscription</a></li>
                <li><img src="../assets/img/buy-comics-shop-locator.png" alt=""><a href="">comic shop locator</a></li>
                <li><img src="../assets/img/buy-dc-power-visa.svg" alt=""><a href="">dc power visa</a></li>
            </ul>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'AppMain'
}
</script>

<style lang="scss" scoped>
.main{
    height: 350px;
}
.main-top{
    height: 50%;
    background-color: black;
    span{
        color: white;
        font-size: 1.5em;
    }
}

.cont-top{
    width: 70%;
    margin: 0 auto;
    display: flex;
    line-height: 150px;
    height: 100%;  
}
.cont-bottom{
    width: 80%;
    margin: 0 auto;
    display: flex;
    line-height: 150px;
    height: 100%; 
    justify-content: space-around;
}


.main-bottom{
    height: 50%;
    background-color: #0080ff;
    ul{
        display: flex;
        img{
            height: 30%;
            vertical-align: middle;
            margin: 1em;
        }
        a{
            text-transform: uppercase;
            color: white;
            font-size: 12px;
        }
    }
}
    
</style>