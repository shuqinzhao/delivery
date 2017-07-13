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

  .main {
    position: fixed;
    top: 70px;
    bottom: 50px;
    left: 40px;
    right: 40px;
    padding: 10px;
    background: #f8f8f8;
  }
</style>
