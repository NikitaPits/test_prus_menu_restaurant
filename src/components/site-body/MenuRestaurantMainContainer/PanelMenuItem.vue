<template>
  <p v-bind:class="[props.panelItemState[props.name.id-1] ? 'btn-cuisune-active':'btn-cuisune']"
      v-on:click="$emit('was-clicked', props.name.id)"
  >
    <slot></slot>

  </p>
</template>

<script setup>
import {defineProps} from "vue";
const props = defineProps({
  name:{value: Object,
    required: true},
  panelItemState:{
    value: Object,
    required:true
    }
})
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
  z-index: 11;
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