<template>
  <div class="home">
    <div class="antd">
      <antd-collapse></antd-collapse>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AntdCollapse from "../components/antd-collapse.vue";

export default defineComponent({
  name: "HomeView",
  components: { AntdCollapse },
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
