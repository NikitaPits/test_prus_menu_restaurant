<template>
  <a
      href="https://www.oblixrestaurant.com"
      class="logo_header logo_header_top">
<site-logotype :color="color"/>
    <div class="text">
      <span>
        {{'at '}}
      </span>
       {{' THE SHARD'}}
    </div>
  </a>
</template>

<script setup>

import SiteLogotype from "@/components/UI/SiteLogotype";
let color ="#fff"
</script>

<style scoped>
.text {
  color: #fff;
  font-family: Muli-ExtraBold;
  font-size: 15px;
  font-weight: 800;
  letter-spacing: .5px;
  position: absolute;
  right: 0;
  text-align: right;
  text-transform: uppercase;
  -webkit-transition: top .3s ease,left .3s ease;
  transition: top .3s ease,left .3s ease;
  white-space: nowrap;
  left: 0;
  top: 100%;
  -webkit-transition-delay: .2s,.2s;
  transition-delay: .2s,.2s;
}
.text span:before{
  border-bottom: 1px solid #fff;
  bottom: -2px;
  content: "";
  height: 100%;
  position: absolute;
  right: 0;
  text-align: center;
  width: 9px;

}
.logo_header_top {
  display: block;
  position: relative;
  margin-right: 60px;
  z-index: 30;
}
.site-header .logo_header_top svg {
  height: 80px;
  width: 180px;
  -webkit-transition-delay: 0s,0s;
  transition-delay: 0s,0s;
}
.site-header .logo_header svg {
  fill: #fff;
  -webkit-transition: width .3s ease,height .3s ease;
  transition: width .3s ease,height .3s ease;
  -webkit-transition-delay: .2s,.2s;
  transition-delay: .2s,.2s;
  height: 47px;
  width: 105px;
}
.logo_header_top svg {
  height: 80px;
  width: 180px;
  -webkit-transition-delay: 0s,0s;
  transition-delay: 0s,0s;
}
a {
  color: inherit;
  cursor: pointer;
  text-decoration: inherit;
  background-color: transparent;
  cursor: pointer;
}
span{
  bottom: 4.5px;
  font-family: Muli-Bold;
  font-size: 9px;
  font-weight: 700;
  letter-spacing: .3px;
  position: relative;
  text-transform: lowercase;
}
</style>