<template>
  <div class="home">
    <h1>This is an home page</h1>
    <a-button>Add</a-button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { Button } from "ant-design-vue";
// const ButtonGroup = Button.Group;

export default defineComponent({
  name: "HomeView",
  components: {
    AButton: Button,
    // AButtonGroup: ButtonGroup,
  },
});
</script>
