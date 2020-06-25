<template>
  <section class="bg-white py-8">
    <div class="container max-w-5xl mx-auto h-12 m-8">
        <swiper ref="mySwiper" :options="swiperOptions" style="height:300px; color:black">
          <swiper-slide>Slide 1 Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sed explicabo eius modi cum sint nam quis dolores. Odio natus nulla, deleniti reprehenderit ex obcaecati, possimus dolorem nesciunt error earum quas.</swiper-slide>
          <swiper-slide>Slide 2</swiper-slide>
          <swiper-slide>Slide 3</swiper-slide>
          <swiper-slide>Slide 4</swiper-slide>
          <swiper-slide>Slide 5</swiper-slide>
          <div class="swiper-pagination" slot="pagination"></div>
        </swiper>
    </div>
  </section>
</template>

<script>
export default {
  name: 'carrousel',
  data() {
    return {
      swiperOptions: {
        pagination: {
          el: '.swiper-pagination'
        },
        // Some Swiper option/callback...
      }
    }
  },
  computed: {
    swiper() {
      return this.$refs.mySwiper.$swiper
    }
  },
  mounted() {
    console.log('Current Swiper instance object', this.swiper)
    this.swiper.slideTo( 100, false)
  }
}
</script>