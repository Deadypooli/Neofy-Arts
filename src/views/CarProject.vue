<template>
  <Header />
  <img :src="img" class="car-image">
  <img :src="imgFront" class="car-image">
  <img :src="imgSide" class="car-image">
  <img :src="imgBack" class="car-image">
  <img :src="imgTop" class="car-image">
</template>

<script>
import Header from '@/components/Header.vue';
import car45 from '@/img/car/new-car-45.webp';
import carFront from '@/img/car/new-car-front.webp';
import carBack from '@/img/car/new-car-back.webp';
import carSide from '@/img/car/new-car-side.webp';
import carTop from'@/img/car/new-car-top.webp';

export default {
  name: 'Proto0',
  components: {
    Header,
  },
  data() {
    return {
      img: car45,
      imgFront: carFront,
      imgBack: carBack,
      imgSide: carSide,
      imgTop: carTop,
    };
  }
};
</script>
