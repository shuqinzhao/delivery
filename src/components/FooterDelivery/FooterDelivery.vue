<template>
  <div class="footer">
    {{ msg }}
  </div>  
</template>

<script>
export default {
  name: 'footer',
  data () {
    return {
      msg: 'footer'
    }
  }
}
</script>

<style scoped>
  .footer {
    position: fixed;
    bottom: 0;
    padding: 15px 40px;
    width: 100%;
    height: 50px;
    color: #fff;
    background: rgba(0, 0, 0, 1);
    z-index: 10;
  }
</style>
