<template>
  <div class="panel-menu__сuisine">
    <div class="menu-items">
    <panel-menu-item
        v-for="name in names"
        :name="name"
        :panelItemState = "panelItemState"
        :key="name.id"
    @was-clicked="refreshMenuItems">
      {{name.name}}
  </panel-menu-item>
  </div>
    <menu-page-main
        :actualName="actualName"
    />
  </div>
</template>

<script setup>
import PanelMenuItem from "@/components/site-body/MenuRestaurantMainContainer/PanelMenuItem";
import {ref} from "vue";
import MenuPageMain from "@/components/site-body/MenuRestaurantMainContainer/MenuPage/MenuPageMain";
let names=[
{name: 'à la carte menu', id: '1'},
{name: 'rose brunch', id: '2'},
      {name: 'cocktails', id: '3'},
      {name: 'desserts', id: '4'},
    ];
let actualName = ref(names[0].name)
let panelItemState = ref([]);
panelItemState.value[0] = true;

    function refreshMenuItems(n){
      for(let i=0; i <= names.length; i++){
        panelItemState.value[i] = false;
      }
      panelItemState.value[n-1] = true;
      actualName.value = names[n-1].name
    }


</script>

<style scoped>

.panel-menu__сuisine{
  justify-content: center;
  margin-bottom: 60px;
  position: relative;
  display: flex;
  flex-direction: column;
}
.menu-items{
  justify-content: center;
  margin-bottom: 60px;
  position: relative;
  display: flex;
}

</style>