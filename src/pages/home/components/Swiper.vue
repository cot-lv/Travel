<template>
<div class="wrapper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl"/>
      </swiper-slide>
      <!-- Optional controls 图片上翻页的点-->
      <div class="swiper-pagination"  slot="pagination"></div>
      <!-- 左右箭头 -->
      <!-- <div class="swiper-button-prev" slot="button-prev"></div>
      <div class="swiper-button-next" slot="button-next"></div> -->
      <div class="swiper-scrollbar"   slot="scrollbar"></div>
    </swiper>
</div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1811/29/2a6b77b6ff72402.jpg_750x200_d4cec568.jpg'
      }, {
        id: '0002',
        imgUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20191/a211765c0bb579b18c6e7d6d75997a48.jpg_750x200_b6921fa6.jpg'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
   .wrapper >>> .swiper-pagination-bullet-active
      background #fff !important
  .wrapper
    overflow hidden
    width 100%
    height 0
    padding-bottom 26.67%
    background-color #eee
    .swiper-img
      width 100%
</style>
