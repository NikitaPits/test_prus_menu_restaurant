<template>
<button v-bind:class="[btnActive? 'btn-active' : 'btn']"
        v-on:mouseover="changeStyle()"
        v-on:mouseleave="changeStyle()">
<slot></slot>
</button>
</template>

<script setup>
import {ref} from "vue";
    let btnActive = ref(false);
    function changeStyle(){
      btnActive.value = !btnActive.value;
}
</script>

<style scoped>
.btn-active{
  background-color: #fff;
  border: 4px solid #fff;
  color: #000;
  cursor: pointer;
  display: inline-block;
  font-family: Muli-ExtraBold;
  font-size: 15px;
  height: auto;
  letter-spacing: .5px;
  max-width: 50%;
  min-width: 180px;
  padding: 12px 7px;
  text-align: center;
  text-transform: uppercase;
  -webkit-transition-duration: .4s;
  transition-duration: .4s;
  -webkit-transition-property: all;
  transition-property: all;
  z-index: 50;
}
.btn{
  background-color: transparent;
  border: 4px solid #fff;
  color: #fff;
  cursor: pointer;
  display: inline-block;
  font-family: Muli-ExtraBold;
  font-size: 15px;
  height: auto;
  letter-spacing: .5px;
  max-width: 50%;
  min-width: 180px;
  padding: 12px 7px;
  text-align: center;
  text-transform: uppercase;
  -webkit-transition-duration: .4s;
  transition-duration: .4s;
  -webkit-transition-property: all;
  transition-property: all;
  z-index: 50;

}
</style>