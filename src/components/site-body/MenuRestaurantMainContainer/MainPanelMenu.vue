<template>
  <div class="panel-menu__сuisine">
    <panel-menu-item
        v-for="name in names"
        :name="name"
        :panelItemState = "panelItemState"
        :key="name.id"
    @was-clicked="refreshMenuItems">
      {{name.name}}
  </panel-menu-item>
  </div>
</template>

<script setup>
import PanelMenuItem from "@/components/site-body/MenuRestaurantMainContainer/PanelMenuItem";
import {ref} from "vue";
let names=[
{name: 'à la carte menu', id: '1'},
{name: 'rose brunch', id: '2'},
      {name: 'Cocktails', id: '3'},
      {name: 'desserts', id: '4'},
    ];
let panelItemState = ref([]);
    function refreshMenuItems(n){
      for(let i=0; i <= names.length; i++){
        panelItemState.value[i] = false;
      }
      panelItemState.value[n-1] = true;
    }

</script>

<style scoped>

.panel-menu__сuisine{
  justify-content: center;
  margin-bottom: 60px;
  position: relative;
  display: flex;
}

</style>