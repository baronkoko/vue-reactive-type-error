<template>
  <div class="slider"></div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { Swiper, SwiperOptions } from "swiper";

export default defineComponent({
  name: "App",
  data: (): {
    options: SwiperOptions;
  } => ({
    options: {},
  }),
  mounted() {
    new Swiper(".slider", this.options);
  },
});
</script>
