<template>
<div class="filter-selector">
  <h6 v-bind:class="[filterVegetarian?'filter-selector-item-active':'filter-selector-item']"
      @click="filterVegetarianClicked()">
    Vegetarian
  </h6>
  <h6 v-bind:class="[filterContainNuts?'filter-selector-item-active':'filter-selector-item']"
      class="filter-selector-item"
      @click="filterContainNutsClicked()">
    Contains Nuts
  </h6>
</div>
</template>

<script setup>
import {ref} from "vue";

let filterVegetarian = ref(false);
let filterContainNuts = ref(false);
function filterVegetarianClicked(){
  filterVegetarian.value=!filterVegetarian.value
}
function filterContainNutsClicked(){
  filterContainNuts.value=!filterContainNuts.value
}
</script>

<style scoped>
.filter-selector{
  color: #a59e9e;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  font-family: Muli-ExtraBold;
  text-transform: uppercase;
}
.filter-selector-item{
  margin-left: 21px;
  cursor: pointer;
}
.filter-selector-item-active{
  margin-left: 21px;
  color: #000000;
  cursor: pointer;
}
</style>