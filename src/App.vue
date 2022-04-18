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
@font-face {
  font-family: "RockwellStd-Light";
  src: local("RockwellStd-Light"),
  url(./fonts/RockwellStd-Light.otf) format("opentype");
}
@font-face {
  font-family: "Muli-ExtraBold";
  src: local("Muli-ExtraBold"),
  url(./fonts/Muli-ExtraBold.ttf) format("truetype");
}
@font-face {
  font-family: "RockwellStd";
  src: local("RockwellStd"),
  url(./fonts/RockwellStd.otf) format("opentype");
}
.main-app{
  font-family: RockwellStd-Light;
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
  -webkit-text-size-adjust: 100%;
}
body{
  margin: 0;
  padding: 0;
}
html{
  margin: 0;
  padding: 0;
  color: #fff;
  font-family: RockwellStd-Light,serif;
}
*, :after, :before{
  box-sizing: inherit;
}
ul {
  display: block;
  list-style-type: disc;
  margin-block-start: 1em;
  margin-block-end: 1em;
  margin-inline-start: 0px;
  margin-inline-end: 0px;
  padding-inline-start: 40px;
}
p {
  display: block;
  margin-block-start: 1em;
  margin-block-end: 1em;
  margin-inline-start: 0px;
  margin-inline-end: 0px;
}
li{
  margin-right: 2%;
}
h3 {
  line-height: 1.26em;
  font-size: 40px;
}
h1, h2, h3, h4, h5, h6 {
  font-weight: 400;
}
h6{
  font-size: 15px;
}
</style>
