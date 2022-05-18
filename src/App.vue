<template>
  <div id="app">
    <!-- header -->
    <AppHeader />

    <!-- main -->
    <main>
      <div class="cont-img">
      </div>
      <AppMain />
    </main>

    <!-- footer -->
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter
  }
}
</script>

<style lang="scss">
@import "./css/common.scss";

.cont-img{
  height: 300px;
  background-image: url('https://www.tomshw.it/images/images/2020/04/fumetti-quarantena-86547.jpg');
}

</style>
