<template>
  <div class="main-description">
  <div class="description-content">
    <p >Enjoy views of West London alongside sophisticated and classic dishes from our rotisserie and grill; all cooked in our open kitchen.</p>
  </div>
    <a class="description-link">
      More about Oblix West
    </a>
  </div>
</template>

<script setup>

</script>

<style scoped>
.description-content{
  margin-right: 21px;
  color: #fff;
  font-family: RockwellStd-Light,serif;
  font-size: 21px;
  font-weight: 300;
  letter-spacing: .023em;
  line-height: 1.5em;
  margin-block-start: 1em;
  margin-block-end: 1em;
  margin-inline-start: 0px;
  margin-inline-end: 0px;
  text-align: justify;
  display: flex;
  justify-content: space-between;
  flex-direction: row;
  max-width: 745px;
  align-items: center;
}
.description-link{
  font-family: Muli-Bold;
  font-size: 15px;
  padding-bottom: 12px;
  position: relative;
  text-transform: uppercase;
  white-space: nowrap;
  color: #fff;
}
.main-description{
  align-items: center;
  display: flex;
  justify-content: space-between;
  margin-bottom: 70px;
  flex-direction: row;
}
.description-link:after {
  background-color: #fff;
  bottom: 0;
  content: "";
  height: 4px;
  left: 0;
  position: absolute;
  right: 0;
}
</style>