<template>
  <a-mentions v-model:value="value" autofocus @select="onSelect">
    <a-mentions-option value="javascript">javascript</a-mentions-option>
    <a-mentions-option value="html">html</a-mentions-option>
    <a-mentions-option value="css">css</a-mentions-option>
  </a-mentions>
</template>
<script lang="ts">
import { defineComponent, ref, watch } from "vue";
export default defineComponent({
  setup() {
    const value = ref<string>("@css");
    watch(value, () => {
      console.log("value", value);
    });
    const onSelect = (option: { value: string }) => {
      console.log("select", option);
    };

    return {
      value,
      onSelect,
    };
  },
});
</script>