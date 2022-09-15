<template>
  <div>
    <header-area />
    <banner-swiper />
    <new-menu />
  </div>
</template>

<script>
import HeaderArea from "../components/HeaderArea.vue";
import BannerSwiper from "../components/BannerSwiper.vue";
import NewMenu from "../components/Home/NewMenu.vue";

export default {
  name: "HomeView",

  components: {
    HeaderArea,
    BannerSwiper,
    NewMenu,
  },
};
</script>
