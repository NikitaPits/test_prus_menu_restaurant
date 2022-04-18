<template>
  <div class="top-title">
<h3 >
  <slot>{{props.actualName}}</slot>
</h3>
  </div>
</template>

<script setup>
import {defineProps } from "vue";

const props = defineProps({
  actualName:{
    type:String,
    required: true
  }
})
</script>

<style scoped>
.top-title{
  color: black;
  margin-bottom: 0;
  margin-right: 30px;
  align-items: center;
  display: flex;
  width: 50%;
  font-family: RockwellStd;
}
</style>