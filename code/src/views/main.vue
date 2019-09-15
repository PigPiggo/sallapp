<template>
  <div>
    <div class="header">
      <div class="avatar"><img :src="avatar" alt="头像"></div>
      <div class="info">
        <h2><img src="@/assets/img/brand@2x.png" v-if="true" alt="品牌">{{name}}</h2>
        <p>取ajax{{description}} / {{deliveryTime}}分钟送达</p>
        <p>supports循环</p>
      </div>
      <div class="bulletin" v-if="true" >{{bulletin}}</div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      name : '' ,
      description : '' ,
      deliveryTime : '' ,
      score : '' ,
      serviceScore : '' ,
      foodScore : '' ,
      rankRate : '' ,
      minPrice : '' ,
      deliveryPrice : '' ,
      ratingCount : '' ,
      sellCount : '' ,
      //公告
      bulletin : '' ,
      supports : {} ,
      avatar : '' ,
      pics : [] ,
      infos : '' ,
    }
  } ,
  created () {
    
  }

}
</script>

<style lang="less">
  .header {
    height : 212px ;
  }
</style>