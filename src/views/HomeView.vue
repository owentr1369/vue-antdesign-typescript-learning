<template>
  <div class="home">
    <div class="antd">
      <antd-tab></antd-tab>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AntdTab from "../components/antd-tab.vue";

export default defineComponent({
  name: "HomeView",
  components: { AntdTab },
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
