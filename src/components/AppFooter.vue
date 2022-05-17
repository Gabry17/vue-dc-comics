<template>
    <div class="footer">
        <div class="foot-top">
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
        <div class="foot-bottom">

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
    background-color: yellow;
}
.foot-top {
    background-image: url("../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    height: calc(100vh - 450px);
    display: flex;
    justify-content: space-around;
    align-items: center;
    overflow: hidden;
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
        margin:1em 2em;
    }
}

.foot-bottom{
    height: 100px;
    background-color: $color-dark-color;
}
</style>