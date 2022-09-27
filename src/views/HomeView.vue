<template>
  <div class="home">
    <div class="antd">
      <antd-form></antd-form>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AntdForm from "../components/antd-form.vue";

export default defineComponent({
  name: "HomeView",
  components: { AntdForm },
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
