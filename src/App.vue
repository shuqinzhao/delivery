<template>
  <div id="app">
    <Topbar></Topbar>

    <div class="main">
      <router-view></router-view>
    </div>
    <FooterDelivery></FooterDelivery>
  </div>
</template>

<script>
import FooterDelivery from './components/FooterDelivery/FooterDelivery.vue'
import Topbar from './components/Topbar/Topbar.vue'
export default {
  name: 'app',
  components: {
    FooterDelivery,
    Topbar
  }
}
</script>

<style scoped>
  @import 'style/core.css';

  #app {
    width: 100%;
    position: fixed;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    overflow: auto;
  }
  .main {
    background: #f8f8f8;
    padding: 70px 40px 50px 40px;
    /* overflow: auto; */
    position: relative;
    z-index: 1;
  }
</style>
