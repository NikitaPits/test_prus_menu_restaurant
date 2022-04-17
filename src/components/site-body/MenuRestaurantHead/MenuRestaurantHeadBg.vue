<template>
  <div class="head__bg">
    <div class="bg__img bg__img_active"
         data-show="true">
  </div>
  </div>
</template>

<script setup>

</script>

<style scoped>
.head__bg{
  background-image: url("../../../assets/menus-1.jpg") ;
  bottom: 0;
  left: 0;
  position: absolute;
  right: 0;
  top: 0;
  background-repeat: no-repeat;
  background-size: cover;
  height: 500px;
  z-index: 1;
}
.head__bg:after{
  background-color: #140906;
  content: "";
  opacity: .35;
}
.bg__img{
  background-size: cover;
  opacity: 0;
  -webkit-transition: opacity 3s ease;
  transition: opacity 3s ease;
  background-position: 24%;
  bottom: 0;
  left: 0;
  position: relative;
  right: 0;
  top: 0;
}

</style>