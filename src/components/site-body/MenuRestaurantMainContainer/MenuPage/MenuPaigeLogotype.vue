<template>
<div class="page-logotype">
  <site-logotype :color="color" class="page-logo-svg"/>
</div>
</template>

<script setup>
import SiteLogotype from "@/components/UI/SiteLogotype";
let color = "#000"
</script>

<style scoped>
.page-logotype:before, .page-logotype:after{
  background-color: #d6d6d6;
  content: "";
  -webkit-box-flex: 1;
  -ms-flex-positive: 1;
  flex-grow: 1;
  height: 2px;
  margin-bottom: 16px;

}
.page-logotype{
  -webkit-box-align: end;
  -ms-flex-align: end;
  align-items: flex-end;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
}
.page-logo-svg{
  color: black;
  fill: black;
  -webkit-transition: width .3s ease,height .3s ease;
  transition: width .3s ease,height .3s ease;
  -webkit-transition-delay: .2s,.2s;
  transition-delay: .2s,.2s;
  height: 47px;
  width: 105px;
  padding-right: 5%;
  padding-left: 5%;
}

</style>