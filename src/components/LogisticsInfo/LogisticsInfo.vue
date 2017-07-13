<template>
  <div class="logisticsInfo">    
    <ul class="info_list">
      <li class="info_list_item" v-for="(item, key) in infoList" v-bind:key="key"> 
        <p class="time">{{ item.time.split(' ')[0] }}</p>
        <p class="time">{{ item.time.split(' ')[1] }}</p>
        <p class="context">{{ item.context }}</p>
      </li>
    </ul>
  </div>  
</template>

<script>
export default {
  name: 'logisticsInfo',
  data () {
    return {
      infoList: [
        {
          'time': '2012-07-07 13:35:14',
          'context': '客户已签收'
        },
        {
          'time': '2012-07-07 09:10:10',
          'context': '离开[北京石景山营业厅]派送中，递送员[温]，电话[]'
        },
        {
          'time': '2012-07-06 19:46:38',
          'context': '到达[北京石景山营业厅]'
        },
        {
          'time': '2012-07-06 15:22:32',
          'context': '离开[北京石景山营业厅]派送中，递送员[温]，电话[]'
        },
        {
          'time': '2012-07-06 15:05:00',
          'context': '到达[北京石景山营业厅]'
        },
        {
          'time': '2012-07-06 13:37:52',
          'context': '离开[北京_同城中转站]发往[北京石景山营业厅]'
        },
        {
          'time': '2012-07-06 12:54:41',
          'context': '到达[北京_同城中转站]'
        },
        {
          'time': '2012-07-06 11:11:03',
          'context': '离开[北京运转中心驻站班组] 发往[北京_同城中转站]'
        },
        {
          'time': '2012-07-06 10:43:21',
          'context': '到达[北京运转中心驻站班组]'
        },
        {
          'time': '2012-07-05 21:18:53',
          'context': '离开[福建_厦门支公司] 发往 [北京运转中心_航空]'
        },
        {
          'time': '2012-07-05 20:07:27',
          'context': '已取件，到达 [福建_厦门支公司]'
        }
      ]
    }
  }
}
</script>

<style>
.info_list {
  position: relative;
  display: block;
  line-height: 32px;
  margin: 10px auto;
  margin-top: 30px;
}
.info_list_item {
  position: relative;
  padding: 10px 20px;
  border: 1px solid #ddd;
  margin-bottom: 10px;
  background: #fff;
}

.info_list_item::before {
  content: '';
  display: inline-block;
  width: 10px;
  height: 10px;
  position: absolute;
  border-radius: 50%;
  background: #ddd;
  left: -15px;
  top: 50%;
  margin-top: -5px;
  z-index: 1;
}
.info_list::after {
  content: '';
  display: inline-block;
  height: 100%;
  position: absolute;
  top: 0;
  left: -10px;
  bottom: -10px;
  border: 1px solid #ddd;
}
</style>
