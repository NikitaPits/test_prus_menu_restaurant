<template>
  <header class="header">
    <div class="header-wrapper">
  <site-header-logo>Logo</site-header-logo>
  <site-header-main-container>
  </site-header-main-container>
    </div>
  </header>
</template>

<script setup>
import SiteHeaderMainContainer from "@/components/site-header/SiteHeaderMainContainer";
import SiteHeaderLogo from "@/components/site-header/SiteHeaderLogo";
console.log(document.documentElement.clientWidth)
</script>

<style scoped>
.header{
  align-items: center;
  background-color: #1f1917;
  position: fixed;
  color: whitesmoke;
  top: 0;
  width: 100%;
  z-index: 30;
  margin: 0;

}
.header-wrapper{
  padding-top: 20px;
  margin-left: 13%;
  margin-right: 13%;
  justify-content: space-between;
  display: flex;
  height: 90px;
}
.header:before{
  bottom: -55px;
  margin: 0;
  padding: 0;
  background-color: #140906;
  content: "";
  left: 0;
  opacity: .25;
  position: absolute;
  right: 0;
  top: 25px;
  -webkit-transition: bottom .3s ease;
  transition: bottom .3s ease;
}

</style>