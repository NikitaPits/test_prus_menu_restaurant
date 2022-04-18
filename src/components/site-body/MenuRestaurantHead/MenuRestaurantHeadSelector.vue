<template>
  <div class="menu-restaurant-head-selector">
    <div class="main-container-selector">
  <div class="selector">
    <h2 class="head-selector-title">
    West
  </h2>
  </div>
    <div class="selector">
  <h2 class="head-selector-title">
    East
  </h2>
    </div>
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
.main-container-selector{
  margin-left: 12%;
  margin-right: 12%;
  display: flex;
  align-items: center;
  z-index: 10;
}
.menu-restaurant-head-selector{
  height: 82px;
  max-width: none;
  z-index: 11;
  display: flex;
  background-color: rgba(20,9,6,.1);
  align-items: center;
}
.head-selector-title{
color: white;
  font-size: 3.125rem;
  z-index: 12;
}
.selector{
  margin-left: 0;
  -webkit-box-align: center;
  position: relative;
  display: flex;
  margin-right: 20px;
  align-items: center;
  z-index: 10;
}
.selector:after {
  background-color: hsla(0,0%,100%,0);
  bottom: 0;
  content: "";
  height: 4px;
  left: 4px;
  position: absolute;
  right: 4px;
  -webkit-transition: background-color .2s ease;
  transition: background-color .2s ease;
  z-index: 10;
}
</style>