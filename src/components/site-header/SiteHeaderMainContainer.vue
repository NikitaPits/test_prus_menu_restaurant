<template>
  <div class="main-container">
  <site-header-main-container-menu-list v-if="needToAdapt"></site-header-main-container-menu-list>
  <my-button
      :needToAdapt="needToAdapt">
    BOOK A TABLE
  </my-button>
    <div class="open-menu-button"
         v-if="!needToAdapt">
      <span></span>
      <span></span>
      <span></span>
    </div>
  </div>
</template>

<script setup>
import MyButton from "@/components/UI/My-button";
import SiteHeaderMainContainerMenuList from "@/components/site-header/SiteHeaderMainContainerMenuList";
import {onMounted,onUnmounted,computed, ref} from "vue";
let needToAdapt = ref(false);
let windowWidth = ref(window.innerWidth)

const onWidthChange = () => windowWidth.value = window.innerWidth
onMounted(() => window.addEventListener('resize', onWidthChange))
onUnmounted(() => window.removeEventListener('resize', onWidthChange))
needToAdapt = computed(() => {
  if (windowWidth.value >= 1060) return true
  if (windowWidth.value < 1060) return false
  return null; // This is an unreachable line, simply to keep eslint happy.
})

</script>
<style scoped>
.main-container{
  display: flex;
  width: 100%;
  justify-content: space-between;
  height: 50px;
  align-items: flex-start;
  z-index: 20;
}
.open-menu-button{
  cursor: pointer;
  height: 25px;
  width: 29px;
  z-index: 29;
  align-items: center;
  display: flex;
  flex-direction: column;
  margin-left: 30px;
  margin-top: 10px;
}
.open-menu-button>span{
  background-color: #fff;
  border-radius: 1px;
  display: block;
  height: 3px;
  margin-top: 5px;
  -webkit-transform-origin: 11%;
  transform-origin: 11%;
  -webkit-transition: width .3s ease,-webkit-transform .3s ease;
  transition: width .3s ease,-webkit-transform .3s ease;
  transition: transform .3s ease,width .3s ease;
  transition: transform .3s ease,width .3s ease,-webkit-transform .3s ease;
  width: 100%;
}
</style>