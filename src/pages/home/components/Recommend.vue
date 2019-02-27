<template>
  <div class="recommend">
    <div class="title">
      <img class="title-img" src="http://img1.qunarzz.com/piao/fusion/1711/16/bfbb9874e8f11402.png">
      热门推荐
    </div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl">
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{ item.desc }}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1505/bb/bb978d0b35e4965c.water.jpg_200x200_d705f205.jpg',
        title: '户部巷',
        desc: '户部巷位于武昌自由路，是一条长150米的百年老巷，其繁华的早点摊群20年经久不衰。清朝时候，这条百米小巷曾因毗邻藩台衙门而得名。 武汉人将用早点，称为“过早”《汉口竹子枝词》。后在别的城市被敷衍甚至忽略的早餐，被武汉人随意而隆重的提升“过年”般“过”的位置。以“小吃”闻名的户部巷”。'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1505/bb/bb978d0b35e4965c.water.jpg_200x200_d705f205.jpg',
        title: '户部巷',
        desc: '户部巷位于武昌自由路，是一条长150米的百年老巷，其繁华的早点摊群20年经久不衰。清朝时候，这条百米小巷曾因毗邻藩台衙门而得名。 武汉人将用早点，称为“过早”《汉口竹子枝词》。后在别的城市被敷衍甚至忽略的早餐，被武汉人随意而隆重的提升“过年”般“过”的位置。以“小吃”闻名的户部巷”。'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1505/bb/bb978d0b35e4965c.water.jpg_200x200_d705f205.jpg',
        title: '户部巷',
        desc: '户部巷位于武昌自由路，是一条长150米的百年老巷，其繁华的早点摊群20年经久不衰。清朝时候，这条百米小巷曾因毗邻藩台衙门而得名。 武汉人将用早点，称为“过早”《汉口竹子枝词》。后在别的城市被敷衍甚至忽略的早餐，被武汉人随意而隆重的提升“过年”般“过”的位置。以“小吃”闻名的户部巷”。'
      }, {
        id: '0004',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1505/bb/bb978d0b35e4965c.water.jpg_200x200_d705f205.jpg',
        title: '户部巷',
        desc: '户部巷位于武昌自由路，是一条长150米的百年老巷，其繁华的早点摊群20年经久不衰。清朝时候，这条百米小巷曾因毗邻藩台衙门而得名。 武汉人将用早点，称为“过早”《汉口竹子枝词》。后在别的城市被敷衍甚至忽略的早餐，被武汉人随意而隆重的提升“过年”般“过”的位置。以“小吃”闻名的户部巷”。'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .recommend
    background #fff
  .title
    margin-top .2rem
    line-height .8rem
    text-indent 0.2rem
    .title-img
      width .3rem
      height .3rem
  .item
    overflow hidden
    display flex
    height 1.9rem
    .item-img
      width 1.7rem
      height 1.7rem
      padding .1rem
    .item-info
      flex 1
      padding .1rem
      min-width 0
      .item-title
        line-height .54rem
        font-size .32rem
        ellipsis()
      .item-desc
        line-height .4rem
        color #ccc
        ellipsis()
      .item-button
        line-height .44rem
        margin-top .16rem
        background #ff9300
        padding 0 .2rem
        border-radius .06rem
        color #fff
</style>
