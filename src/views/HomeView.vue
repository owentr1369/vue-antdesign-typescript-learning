<template>
  <div class="home">
    <h1>This is an home page</h1>
    <antd-pagination></antd-pagination>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AntdPagination from "@/components/antd-pagination.vue";

export default defineComponent({
  components: { AntdPagination },
  name: "HomeView",
});
</script>
