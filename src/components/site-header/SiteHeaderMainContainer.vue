<template>
  <div class="main-container">
  <site-header-main-container-menu-list v-if="needToAdapt"></site-header-main-container-menu-list>
  <my-button>BOOK A TABLE
  </my-button>
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
</style>