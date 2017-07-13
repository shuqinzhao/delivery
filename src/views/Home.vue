<template>
  <div class="home">
    <SearchDelivery></SearchDelivery>
  </div>  
</template>

<script>
import SearchDelivery from '../components/SearchDelivery/SearchDelivery.vue'
export default {
  name: 'home',
  data () {
    return {
      msg: 'Home'
    }
  },
  components: {
    SearchDelivery
  }
}
</script>
<style scoped>

</style>
