<template>
  <p v-bind:class="[itemActive&&!props.reset ? 'btn-cuisune-active':'btn-cuisune']"
      v-on:click="changeStyle()"
  >
    <slot></slot>

  </p>
  <div>{{props.reset}}</div>
  <div>{{itemActive}}</div>
</template>

<script setup>
import {ref} from "vue";
import {defineProps} from "vue";
const props = defineProps({
  reset:{value: String,
    required: true}})
let itemActive = ref(false)

function changeStyle(){
itemActive.value = !itemActive.value;
  if(props.reset){
    itemActive.value = false
    console.log('itemActive.value')
  }
}


</script>

<style scoped>
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
.btn-cuisune-active {
  border: 4px solid #fff;
  cursor: pointer;
  font-family: Muli-ExtraBold;
  margin-bottom: 10px;
  margin-left: 4px;
  margin-right: 4px;
  opacity: 1;
  padding: 24px 20px;
  text-align: center;
  text-transform: uppercase;
  -webkit-transition: opacity .5s ease,-webkit-transform .5s ease;
  transition: opacity .5s ease,transform .5s ease,-webkit-transform .5s ease;
  z-index: 30;
}
</style>