<template>
  <div id="app">
    <!-- header -->
    <AppHeader />

    <!-- main -->
    <main class="main"></main>

    <!-- footer -->
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter
  }
}
</script>

<style lang="scss">
@import "./css/common.scss";
.main{
  background-color: aqua;
  height: 250px;
}

</style>
