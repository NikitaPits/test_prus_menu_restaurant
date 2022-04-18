<template>
<div class="menu-main-page">
  <menu-paige-logotype/>
  <menu-page-top :actualName="props.actualName"
  />
  <div>{{actualName}}</div>
</div>
</template>

<script setup>
import MenuPaigeLogotype from "@/components/site-body/MenuRestaurantMainContainer/MenuPage/MenuPaigeLogotype";
import MenuPageTop from "@/components/site-body/MenuRestaurantMainContainer/MenuPage/MenuPageTop";
import {defineProps} from "vue";
const props = defineProps({
  actualName:{
    type: String,
    required: true
  }
})
</script>

<style scoped>
.menu-main-page{
  background-color: white;
  padding: 48px 70px 70px;
  display: flex;
  flex-direction: column;
}
.test{
  color: black;
}

</style>