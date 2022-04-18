<template>
  <ul class="menu-list">
    <menu-link>East</menu-link>
    <menu-link>West</menu-link>
    <menu-link>Menus</menu-link>
    <menu-link>Oblix Experiences</menu-link>
    <menu-link>Gift Vouchers</menu-link>
  </ul>
</template>

<script setup>
import MenuLink from "@/components/site-header/MenuLink";
</script>

<style scoped>
.menu-list{
  display: flex;
  justify-content: flex-end;
  width: 100%;
  padding: 0;
  margin-right: 5%;
  align-items: center;
}
</style>