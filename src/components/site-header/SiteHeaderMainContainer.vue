<template>
  <div class="main-container">
  <site-header-main-container-menu-list></site-header-main-container-menu-list>
  <my-button>BOOK A TABLE
  </my-button>
  </div>
</template>

<script setup>
import MyButton from "@/components/UI/My-button";
import SiteHeaderMainContainerMenuList from "@/components/site-header/SiteHeaderMainContainerMenuList";

</script>

<style scoped>
.main-container{
  display: flex;
  width: 100%;
  justify-content: space-between;
  height: 50px;
  align-items: flex-start;
  z-index: 20;
}
</style>