<template>
<div class="menu-restaurant-main-container">
  <main-description/>
  <main-panel-menu/>
</div>
</template>

<script>
import MainDescription from "@/components/site-body/MenuRestaurantMainContainer/MainDescription";
import MainPanelMenu from "@/components/site-body/MenuRestaurantMainContainer/MainPanelMenu";
export default {
  components: {MainPanelMenu, MainDescription}
}
</script>

<style scoped>
.menu-restaurant-main-container{
  padding-bottom: 91px;
  padding-top: 70px;
  margin-left: 70px;
  margin-right: 70px;
}
</style>