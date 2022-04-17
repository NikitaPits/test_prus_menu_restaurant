<template>
<div class="main-app">
  <SiteHeader/>
  <SiteContent></SiteContent>
</div>
</template>

<script>

import SiteContent from "@/components/site-body/SiteContent";
import SiteHeader from "@/components/site-header/SiteHeader";

export default {
  name: 'App',
  components: {
    SiteHeader,
    SiteContent,
  }
}
</script>

<style>
.main-app{
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  background-color: #1f1917;
}
.test {
  padding: 5px;
  margin: 5px;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
  margin-top: 60px;
}
body{
  margin: 0;
  padding: 0;
}
html{
  margin: 0;
  padding: 0;
}
</style>
