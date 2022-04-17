<template>
  <div class="main-container">
  <site-header-main-container-menu-list class="test main-container"></site-header-main-container-menu-list>
  <my-button>
  </my-button>
  </div>
</template>

<script setup>
import MyButton from "@/components/UI/My-button";
import SiteHeaderMainContainerMenuList from "@/components/site-header/SiteHeaderMainContainerMenuList";

</script>

<style scoped>
.main-container{
  color: whitesmoke;
  display: flex;
  justify-content:space-between;
}

</style>