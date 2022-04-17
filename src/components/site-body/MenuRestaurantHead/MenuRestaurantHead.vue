<template>
  <div class="menu-restaurant-header">
<menu-restaurant-head-bg/>
  <menu-restaurant-head-title/>
    <menu-restaurant-head-selector/>
  </div>
</template>

<script setup>
import MenuRestaurantHeadBg from "@/components/site-body/MenuRestaurantHead/MenuRestaurantHeadBg";
import MenuRestaurantHeadTitle from "@/components/site-body/MenuRestaurantHead/MenuRestaurantHeadTitle";
import MenuRestaurantHeadSelector from "@/components/site-body/MenuRestaurantHead/MenuRestaurantHeadSelector";
</script>

<style scoped>
.menu-restaurant-header{
  height: 500px;
  display: flex;
  justify-content: flex-end;
  flex-direction: column;
  background-position: 24%;
  position: relative;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
}
</style>