<style scoped>
  .swiper-slide {
    width: 250px;
  }
</style>

<template>
  <div>
    <div class="btn-group btn-vue-example">
      <button class="btn btn-default btn-xs btn-title">scrollbar</button>
      <button class="btn btn-default btn-xs btn-title">滚动条</button>
      <a href="https://github.com/surmon-china/vue-awesome-swiper/blob/master/examples/13-scrollbar.vue" target="_blank" class="btn btn-primary btn-xs">&lt; &gt;</a>
    </div>
    <swiper :options="swiperOption">
      <swiper-slide>Slide 1</swiper-slide>
      <swiper-slide>Slide 2</swiper-slide>
      <swiper-slide>Slide 3</swiper-slide>
      <swiper-slide>Slide 4</swiper-slide>
      <swiper-slide>Slide 5</swiper-slide>
      <swiper-slide>Slide 6</swiper-slide>
      <swiper-slide>Slide 7</swiper-slide>
      <swiper-slide>Slide 8</swiper-slide>
      <swiper-slide>Slide 9</swiper-slide>
      <swiper-slide>Slide 10</swiper-slide>
      <div class="swiper-scrollbar" slot="scrollbar"></div>
    </swiper>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        swiperOption: {
          scrollbar: '.swiper-scrollbar',
          scrollbarHide: true,
          slidesPerView: 'auto',
          centeredSlides: true,
          spaceBetween: 30,
          grabCursor: true
        }
      }
    }
  }
</script>
