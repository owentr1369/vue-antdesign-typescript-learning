<template>
  <div class="home">
    <h1>This is an home page</h1>
    <antd-button></antd-button>
  </div>
</template>

<script lang="ts">
import antdButton from "@/components/antd-button.vue";
import { defineComponent } from "vue";

export default defineComponent({
  components: { antdButton },
  name: "HomeView",
});
</script>
