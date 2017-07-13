<template>
  <div class="home">
    <SearchDelivery></SearchDelivery>

    <LogisticsInfo></LogisticsInfo>
  </div>  
</template>

<script>
import SearchDelivery from '../components/SearchDelivery/SearchDelivery.vue'
import LogisticsInfo from '../components/LogisticsInfo/LogisticsInfo.vue'

export default {
  name: 'home',
  data () {
    return {
      msg: 'Home'
    }
  },
  components: {
    SearchDelivery,
    LogisticsInfo
  }
}
</script>
<style scoped>

</style>
