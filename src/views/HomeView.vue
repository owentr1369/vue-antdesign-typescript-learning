<template>
  <div class="home">
    <div class="antd">
      <antd-auto-complete></antd-auto-complete>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AntdAutoComplete from "../components/antd-auto-complete.vue";

export default defineComponent({
  components: { AntdAutoComplete },
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
