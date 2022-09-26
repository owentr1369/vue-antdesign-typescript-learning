<template>
  <div class="home">
    <h1>This is an home page</h1>
    <antd-dropdown></antd-dropdown>
  </div>
</template>

<script lang="ts">
import AntdDropdown from "@/components/antd-dropdown.vue";
import { defineComponent } from "vue";

export default defineComponent({
  components: { AntdDropdown },
  name: "HomeView",
});
</script>
