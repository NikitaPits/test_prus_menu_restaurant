<template>
  <div class="main-container">
  <site-header-main-container-menu-list class="menu-list"></site-header-main-container-menu-list>
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
  color: whitesmoke;
  display: flex;
  align-items: center;
  justify-items: flex-end;
  left: 0;
  position: relative;
  width: 100%;
}
.menu-list{
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-flex: 1;
  -ms-flex: 1;
  flex: 1;
  -webkit-box-pack: end;
  -ms-flex-pack: end;
  justify-content: flex-end;
  width: 100%;
}

</style>