<template>
<div class="main">
    <div class="main-top">
        <div class="cont-top">
            <button class="btn-1">current series</button>
            <div class="cont-props">
                <AppProps 
                v-for="(element,index) in image" 
                :key="index"
                :productObj="element" />
            </div>
            <button class="btn-2">Load More</button>
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
import AppProps from "./AppProps.vue";

export default {
    name: 'AppMain',
    components: {
      AppProps,
    },
    data: function(){
        return{
            image:[
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {   
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                  "price": "$3.99",
                  "series": "American Vampire 1976",
                  "type": "comic book"
                },
                {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                  "price": "$16.99",
                  "series": "Aquaman",
                  "type": "graphic novel"
                },
                {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                  "price": "$2.99",
                  "series": "Batgirl",
                  "type": "comic book"
                },
                {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                  "price": "$3.99",
                  "series": "Batman",
                  "type": "comic book"
                },
                {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                  "price": "$2.99",
                  "series": "Batman Beyond",
                  "type": "comic book"
                },
                {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                  "price": "$3.99",
                  "series": "Batman/Superman",
                  "type": "comic book"
                },
                {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                  "price": "$4.99",
                  "series": "Batman/Superman Annual",
                  "type": "comic book"
                },
                {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                  "price": "$5.99",
                  "series": "Batman: The Joker War Zone",
                  "type": "comic book"
                },
                {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                  "price": "$6.99",
                  "series": "Batman: Three Jokers",
                  "type": "comic book"
                },
                {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                  "price": "$4.99",
                  "series": "Batman: White Knight Presents: Harley Quinn",
                  "type": "comic book"
                },
                {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                  "price": "$16.99",
                  "series": "Catwoman",
                  "type": "graphic novel"
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../css/variables';
@mixin styleBtn{
    border: none;
    background-color: $color-primary-color;
    padding: 1em 2em;
    color: $color-text-color;
    text-transform: uppercase;
}

.main-top{
    background-color: black;
    span{
        color: $color-text-color;
        font-size: 1.5em;
    }
}

.cont-top{
    width: 70%;
    margin: 0 auto;
    text-align: center;
    padding-bottom: 1em;
    position: relative;
    .btn-1{
        position: absolute;
        top: -20px;
        left: 0;
        @include styleBtn()
    }
    .cont-props{
        color: $color-text-color;
        display: flex;
        flex-wrap: wrap;
        padding-top: 3em;
    }
    .btn-2{
        @include styleBtn()
    }
}

.cont-bottom{
    width: 80%;
    margin: 0 auto;
    display: flex; 
    justify-content: space-around;
}


.main-bottom{
    background-color: $color-primary-color;
    ul{
        display: flex;
        padding: 3em 0;
        img{
            height: 50px;
            vertical-align: middle;
            margin: 1em;
        }
        a{
            text-transform: uppercase;
            color: $color-text-color;
            font-size: 12px;
        }
    }
}
    
</style>