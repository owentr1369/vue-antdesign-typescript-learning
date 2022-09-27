<template>
  <div class="home">
    <div class="antd">
      <antd-slider></antd-slider>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AntdSlider from "../components/antd-slider.vue";

export default defineComponent({
  name: "HomeView",
  components: { AntdSlider },
});
</script>

<style lang="scss">
.home {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 70vh;
  overflow: hidden;
  flex-direction: column;
  .antd {
    width: 60%;
    height: 100%;
  }
}
</style>
