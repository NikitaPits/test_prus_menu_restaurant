<template>
  <li v-bind:class="[linkActive? 'menu-link-active': 'menu-link']"
      v-on:mouseleave="changeStyle()"
      v-on:mouseover="changeStyle()">
  <slot></slot>
  </li>
</template>

<script setup>
import {ref} from "vue";

    let linkActive = ref(false);
    function changeStyle(){
      linkActive.value = !linkActive.value;
}
</script>

<style scoped>
.menu-link{
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  color: #a59e9e;
  cursor: pointer;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  font-family: RockwellStd;
  font-size: 18px;
  font-weight: 400;
  letter-spacing: .007em;
  line-height: 1em;
  vertical-align: middle;
  width: 100%;
  margin-right: 41px;
  z-index: 30;
  text-align: justify;
}
.menu-link-active{
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  color: #fff;
  cursor: pointer;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  font-family: RockwellStd;
  font-size: 18px;
  font-weight: 400;
  letter-spacing: .007em;
  line-height: 1em;
  vertical-align: middle;
  width: 100%;
  margin-right: 41px;
  z-index: 30;
  text-align: justify;
}
</style>