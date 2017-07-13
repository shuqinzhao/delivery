<template>
  <div class="searchDelivery">    
    <div class="search">
      <p class="search_text">快递智能查询 </p>
      <input type="text" class="search_input" v-model="tracking_number" placeholder="请输入快递单号" />
      <button class="search_btn">查询</button>
    </div>
    {{ tracking_number }}
  </div>  
</template>

<script>
export default {
  name: 'searchDelivery',
  data () {
    return {
      msg: 'searchDelivery',
      tracking_number: ''
    }
  }
}
</script>

<style>
.search {
  text-align: center;
  margin-top: 30px;
  font-weight: bold;
  margin: 0 auto;
}
.search_text {
  padding: 10px;
  margin-bottom: 10px;
}
.search_input {
  height: 35px;
  padding: 5px 10px;
  width: 75%;
  display: inline-block;
}
.search_btn {
  height: 35px;
  width: 20%;
  text-align: center;
  background: rgba(0, 0, 0, 0.8);
  color: #fff;
  box-shadow: none;
  outline: none;
  border: none;
}
</style>
