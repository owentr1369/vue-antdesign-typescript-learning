<template>
  <a-pagination
    v-model:current="current"
    :total="500"
    :showQuickJumper="true"
  />
</template>
<script lang="ts">
import { defineComponent, ref } from "vue";
export default defineComponent({
  setup() {
    return {
      current: ref(6),
    };
  },
});
</script>