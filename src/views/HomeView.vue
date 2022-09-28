<template>
  <div class="home">
    <div class="antd">
      <antd-empty></antd-empty>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AntdEmpty from "../components/antd-empty.vue";

export default defineComponent({
  name: "HomeView",
  components: { AntdEmpty },
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
