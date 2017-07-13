<template>
  <div class="topbar">
    <img src='../../assets/logo.png' />
  </div>  
</template>

<script>
export default {
  name: 'topbar',
  data () {
    return {
      msg: 'topbar'
    }
  }
}
</script>

<style scoped>
  .topbar {
    position: fixed;
    top: 0;
    padding: 10px 40px;
    width: 100%;
    height: 70px;
    color: #fff;
    background: #000;
    opacity: 0.8;
    z-index: 10;
  }
</style>
