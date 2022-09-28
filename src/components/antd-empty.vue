<template>
  <a-empty />
  <br /><br />
  <a-empty :image="simpleImage" />
  <br /><br />
  <a-empty
    image="https://gw.alipayobjects.com/mdn/miniapp_social/afts/img/A*pevERLJC9v0AAAAAAAAAAABjAQAAAQ/original"
    :image-style="{
      height: '60px',
    }"
  >
    <template #description>
      <span>
        Customize
        <a href="#API">Description</a>
      </span>
    </template>
    <a-button type="primary">Create Now</a-button>
  </a-empty>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { Empty } from "ant-design-vue";
export default defineComponent({
  setup() {
    return {
      simpleImage: Empty.PRESENTED_IMAGE_SIMPLE,
    };
  },
});
</script>