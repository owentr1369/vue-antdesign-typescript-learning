<template>
  <div class="home">
    <div class="antd">
      <antd-date-picker></antd-date-picker>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AntdDatePicker from "../components/antd-date-picker.vue";

export default defineComponent({
  name: "HomeView",
  components: { AntdDatePicker },
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
