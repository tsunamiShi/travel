<template>
    <div class="wrapper">
        <swiper :options="swiperOption">
            <swiper-slide v-for="item of swiperList" :key="item.id">
                <img class="swiper-img" :src="item.imgUrl">
            </swiper-slide>
            <div class="swiper-pagination"  slot="pagination"></div>
        </swiper>
    </div>
</template>

<script>
export default {
  name: "HomeSwiper",
  data() {
    return {
      swiperOption: {
          pagination: '.swiper-pagination',
          loop: true
      },
      swiperList: [{
          id: '0001',
          imgUrl: '/static/img/bca92895556c5002.jpg_750x200_cf56d46c.jpg'
      }, {
          id: '0002',
          imgUrl: '/static/img/ba3c1ad4fa21ae02.jpg_750x200_a76690c1.30bc204.jpg'
      }]
    };
  }
};
</script>

<style lang="stylus" scoped>
    .wrapper >>> .swiper-pagination-bullet-active
        background #fff
    .wrapper
        overflow hidden
        width 100%
        height 0
        padding-bottom 26.7%
        background #eee
        .swiper-img 
            width 100%

</style>
