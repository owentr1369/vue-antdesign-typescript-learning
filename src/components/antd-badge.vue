<template>
  <div class="antd-badge">
    <a-badge :count="99">
      <a-avatar shape="square" size="large" />
    </a-badge>
    <a-badge :count="100">
      <a-avatar shape="square" size="large" />
    </a-badge>
    <a-badge :count="99" :overflow-count="10">
      <a-avatar shape="square" size="large" />
    </a-badge>
    <a-badge :count="1000" :overflow-count="999">
      <a-avatar shape="square" size="large" />
    </a-badge>
  </div>
</template>

<style lang="scss" scoped>
.antd-badge {
  display: flex;
  justify-content: space-around;
}
</style>