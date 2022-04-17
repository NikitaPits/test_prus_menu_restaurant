<template>
  <div class="panel-menu__сuisine"
  v-on:click="clearStyles()">
    <panel-menu-item
        :reset="needToClear">
    à la carte menu
  </panel-menu-item>
    <panel-menu-item
        :reset="needToClear">
    rose brunch
  </panel-menu-item>
    <panel-menu-item
        :reset="needToClear">
    Cocktails
  </panel-menu-item>
    <panel-menu-item
        :reset="needToClear">
    desserts
  </panel-menu-item>
  </div>
</template>

<script setup>
import PanelMenuItem from "@/components/site-body/MenuRestaurantMainContainer/PanelMenuItem";
import {ref} from "vue";
    let needToClear = ref(false);
   function clearStyles(){
      needToClear.value = true
     function reset(){
       needToClear.value = false
     }
     setTimeout(reset,1000 )
    }

</script>

<style scoped>

.panel-menu__сuisine{
  justify-content: center;
  margin-bottom: 60px;
  position: relative;
  display: flex;
}
.btn-cuisune {
  border: 4px solid #fff;
  cursor: pointer;
  font-family: Muli-ExtraBold;
  margin-bottom: 10px;
  margin-left: 4px;
  margin-right: 4px;
  opacity: .2;
  padding: 24px 20px;
  text-align: center;
  text-transform: uppercase;
  -webkit-transition: opacity .5s ease,-webkit-transform .5s ease;
  transition: opacity .5s ease,transform .5s ease,-webkit-transform .5s ease;
}
</style>