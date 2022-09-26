<template>
  <div class="demo-dropdown-wrap">
    <a-dropdown-button @click="handleButtonClick">
      Dropdown
      <template #overlay>
        <a-menu @click="handleMenuClick">
          <a-menu-item key="1">
            <UserOutlined />
            1st menu item
          </a-menu-item>
          <a-menu-item key="2">
            <UserOutlined />
            2nd menu item
          </a-menu-item>
          <a-menu-item key="3">
            <UserOutlined />
            3rd item
          </a-menu-item>
        </a-menu>
      </template>
    </a-dropdown-button>
    <a-dropdown-button>
      Dropdown
      <template #overlay>
        <a-menu @click="handleMenuClick">
          <a-menu-item key="1">
            <UserOutlined />
            1st menu item
          </a-menu-item>
          <a-menu-item key="2">
            <UserOutlined />
            2nd menu item
          </a-menu-item>
          <a-menu-item key="3">
            <UserOutlined />
            3rd item
          </a-menu-item>
        </a-menu>
      </template>
      <template #icon><UserOutlined /></template>
    </a-dropdown-button>
    <a-dropdown-button disabled @click="handleButtonClick">
      Dropdown
      <template #overlay>
        <a-menu @click="handleMenuClick">
          <a-menu-item key="1">
            <UserOutlined />
            1st menu item
          </a-menu-item>
          <a-menu-item key="2">
            <UserOutlined />
            2nd menu item
          </a-menu-item>
          <a-menu-item key="3">
            <UserOutlined />
            3rd item
          </a-menu-item>
        </a-menu>
      </template>
    </a-dropdown-button>
    <a-dropdown>
      <template #overlay>
        <a-menu @click="handleMenuClick">
          <a-menu-item key="1">
            <UserOutlined />
            1st menu item
          </a-menu-item>
          <a-menu-item key="2">
            <UserOutlined />
            2nd menu item
          </a-menu-item>
          <a-menu-item key="3">
            <UserOutlined />
            3rd item
          </a-menu-item>
        </a-menu>
      </template>
      <a-button>
        Button
        <DownOutlined />
      </a-button>
    </a-dropdown>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { UserOutlined, DownOutlined } from "@ant-design/icons-vue";
import type { MenuProps } from "ant-design-vue";

export default defineComponent({
  components: {
    UserOutlined,
    DownOutlined,
  },
  setup() {
    const handleButtonClick = (e: Event) => {
      console.log("Click left button", e);
    };
    const handleMenuClick: MenuProps["onClick"] = (e) => {
      console.log("Click", e);
    };
    return {
      handleButtonClick,
      handleMenuClick,
    };
  },
});
</script>
