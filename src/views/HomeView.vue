<template>
  <div class="home">
    <div class="antd">
      <antd-time-picker></antd-time-picker>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AntdTimePicker from "../components/antd-time-picker.vue";

export default defineComponent({
  name: "HomeView",
  components: { AntdTimePicker },
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
