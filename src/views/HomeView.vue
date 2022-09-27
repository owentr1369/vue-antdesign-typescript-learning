<template>
  <div class="home">
    <div class="antd">
      <antd-mention></antd-mention>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AntdMention from "../components/antd-mention.vue";

export default defineComponent({
  name: "HomeView",
  components: { AntdMention },
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
