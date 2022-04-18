<template>
  <h6 class="filter-title">FILTER BY:</h6>
<top-filter-selector/>
</template>

<script>
import TopFilterSelector
  from "@/components/site-body/MenuRestaurantMainContainer/MenuPage/MenuPageTopItems/TopFilterSelector";
export default {
  name: "TopFilter",
  components: {TopFilterSelector}
}
</script>

<style scoped>
.filter-title{
  color: black;
  font-family: Muli-ExtraBold;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>