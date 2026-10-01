<template>
  <Header />
    <div class="main-image" :style="{backgroundImage: 'url(' + img + ')' }">
        <h1 class="main-text">
            <span>N</span><span>E</span><span>O</span><span>F</span><span>Y</span>
        </h1>
    </div>
</template>

<script>
import Header from '@/components/Header.vue';
import img from '@/img/personal/Skye-Wallpaper.webp';

export default {
  name: 'Index',
  components: {
    Header,
  },
  data() {
    return {
      img: img,
    };
  }
};
</script>
