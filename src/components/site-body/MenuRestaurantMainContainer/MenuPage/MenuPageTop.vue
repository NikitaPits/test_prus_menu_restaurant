<template>
  <div class="menu-page-top">
    <top-title :actualName="props.actualName"/>
    <top-filter/>
  </div>
</template>

<script setup>
import TopTitle from "@/components/site-body/MenuRestaurantMainContainer/MenuPage/MenuPageTopItems/TopTitle";
import TopFilter from "@/components/site-body/MenuRestaurantMainContainer/MenuPage/MenuPageTopItems/TopFilter";
import {defineProps} from "vue";
const props = defineProps({
  actualName:{
    type: String,
    required: true
  }
})

</script>

<style scoped>
.menu-page-top{
  display: flex;
  justify-content: space-between;
}
</style>