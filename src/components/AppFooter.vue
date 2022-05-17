<template>
    <div class="footer">
        <div class="foot-top">
            <div class="top">
                <div class="link">
                <div>
                    <ul>
                    <li><h3>dc comics</h3></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                </ul>
                <ul>
                    <li><h3>shop</h3></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                </ul>
                </div>
                <ul>
                    <li><h3>dc</h3></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                </ul>
                <ul>
                    <li><h3>sites</h3></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                    <li><a href="">ciao</a></li>
                </ul>
            </div>
            <div class="img">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
            </div>
        </div>
        <div class="foot-bottom">
            <div class="text">
                <div class="button">
                    <button>sign-up now</button>
                </div>
                <div class="icon">
                    <span>follow us</span>
                    <img src="../assets/img/footer-facebook.png" alt="">
                    <img src="../assets/img/footer-periscope.png" alt="">
                    <img src="../assets/img/footer-twitter.png" alt="">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                    <img src="../assets/img/footer-youtube.png" alt="">
                </div>
            </div>
        </div>
        
    </div>
</template>

<script>
export default {
    name: 'AppFooter'
}
</script>

<style lang="scss" scoped>
$color-dark-color: #212121;
.footer {
    height: calc(100vh - 450px);
}
.foot-top {
    background-image: url("../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    overflow: hidden;
    height: 80%;
    li {
        a{
            color: #8f8c8c;
        }
        h3 {
            color: white;
            text-transform: uppercase;
            margin-bottom: 1em;
        }
    }
}

.link{
    display: flex;
    ul{
        margin-right: 1em;
        margin-top: 1em;
    }
}

.top{
    width: 70%;
    height: 100%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}


.foot-bottom{
    height: 20%;
    background-color: $color-dark-color;
    .text{
        width: 70%;
        height: 100%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        button{
            color: white;
            background-color: inherit;
            border: 1px solid #0080ff;
            padding: 1em;
        }
    }

    .icon{
        span{
            color: #0080ff;
            text-transform: uppercase;
            vertical-align: middle;
        }
        img{
            margin-left: 1em;
            vertical-align: middle;
        }
    }
}
</style>