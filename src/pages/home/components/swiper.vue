<template>
  <div class="swiper">
    <swiper :options="swiperOptions">
      <swiper-slide v-for="item of list" :key="item.id">
        <img class="swiper-img" :src="item.img"/>
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOptions: {
        // autoplay: 3000,
        pagination: '.swiper-pagination',
        paginationClickable: true,
        loop: true
      },
      list: [
        {
          id: '1000',
          img: 'https://source.qunarzz.com/site/images/wns/20200630_qunar_dujia_750x192_3.jpg'
        },
        {
          id: '2000',
          img: 'https://source.qunarzz.com/site/images/wns/20200608_qunar_dujia_750x192_1.jpg'
        }
      ]
    }
  }
}
</script>
<style lang="stylus" scoped>
  .swiper >>> .swiper-pagination-bullet-active
    background-color #ffffff !important

  .swiper
    width 100%
    height 25.6vw

    .swiper-img
      width 100%
</style>
