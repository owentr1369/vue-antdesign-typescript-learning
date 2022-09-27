<template>
  <div class="home">
    <div class="antd">
      <antd-steps></antd-steps>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AntdSteps from "@/components/antd-steps.vue";

export default defineComponent({
  components: { AntdSteps },
  name: "HomeView",
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
