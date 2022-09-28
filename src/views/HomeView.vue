<template>
  <div class="home">
    <div class="antd">
      <antd-timeline></antd-timeline>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AntdTimeline from "../components/antd-timeline.vue";

export default defineComponent({
  name: "HomeView",
  components: { AntdTimeline },
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
