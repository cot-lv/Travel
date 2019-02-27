<template>
  <div class="weekend">
    <div class="title">周末去哪儿</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl">
        </div>
        <div class="item-info">
          <p class="item-title">{{ item.title }}</p>
          <p class="item-desc">{{ item.desc }}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1505/d5/abe8a48a6ef8bf.jpg_r_640x214_7c41cc81.jpg',
        title: '武汉必打卡',
        desc: '到武汉感受神奇的热干面之都'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1711/4f/59f533696344fe.jpg_r_640x214_f8aa8c8f.jpg',
        title: '湖北泡汤胜地',
        desc: '一边赏美景一边泡温泉过冬日，这里有最全最优惠的泡汤圣地，让你美美的过个冬日'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1811/6d/5afbf529076ef6.jpg_r_640x214_7414b151.jpg',
        title: '三峡人家',
        desc: '感受长江的水三峡的情怀，自古至今，无数骚人墨客浓墨重彩的描绘三峡，赶紧领略三峡的壮美吧！'
      }, {
        id: '0004',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1505/4f/95a94c90ef3521.jpg_r_640x214_345412f9.jpg',
        title: '开启亲子时光',
        desc: '远离喧嚣的都市，带孩子去一个幽静，清新的天然“氧吧”，呼吸新鲜空气，亲近自然健康成长'
      }, {
        id: '0005',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1507/e0/4aae49007c8a64.jpg_r_640x214_65a42783.jpg',
        title: '周末出游乐翻天',
        desc: '周末，想去哪儿就去哪儿~'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .weekend
    background #fff
  .title
    margin-top .2rem
    line-height .8rem
    text-indent 0.2rem
  .title-img
    width .3rem
    height .3rem
  .item-img-wrapper
    overflow hidden
    height 0
    padding-bottom 33.9%
  .item-img
    width 100%
  .item-info
    padding .2rem
    .item-title
      line-height .48rem
      font-size .28rem
      color #212121
      ellipsis()
    .item-desc
      line-height .42rem
      color #616161
      font-size .24rem
      ellipsis()
</style>
