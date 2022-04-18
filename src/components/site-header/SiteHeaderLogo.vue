<template>
  <a
      href="https://www.oblixrestaurant.com"
      class="logo_header logo_header_top">
    <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 107.941 48.489">
      <g data-name="Group 1409">
        <path data-name="Path 1087"
              d="M12.02 24.449a12.02 12.02 0 1 0 12.02 12.02 12.02 12.02 0 0 0-12.02-12.02zm0 21.093a9.074 9.074 0 1 1 9.074-9.074 9.074 9.074 0 0 1-9.074 9.074z"
              fill="#fff">
        </path>

        <path
            data-name="Path 1088"
            d="M40.301 24.449a12.02 12.02 0 1 0 12.02 12.02 12.02 12.02 0 0 0-12.02-12.02zm0 21.093a9.074 9.074 0 1 1 9.074-9.074 9.074 9.074 0 0 1-9.074 9.074z"
            fill="#fff">
        </path>
        <path
            data-name="Rectangle 1572"
            fill="#fff"
            d="M81.795 26.514l2.225-2.225 21.931 21.93-2.225 2.226z">
        </path>
        <path
            data-name="Rectangle 1573"
            fill="#fff"
            d="M69.643 24.331h5.774v24.157h-5.774z">

        </path>
        <path
            data-name="Rectangle 1574"
            fill="#fff"
            d="M56.916.057h5.774v48.432h-5.774z">

        </path>
        <path
            data-name="Rectangle 1575"
            fill="#fff"
            d="M84.019 48.445l-2.225-2.225 21.93-21.931 2.226 2.225z">

        </path>
        <path
            data-name="Line 211"
            fill="none"
            d="M71.293 24.275h36.648">

        </path>
        <path
            data-name="Line 212"
            fill="none"

            d="M59.391 0H23.332">

        </path>
        <path
            data-name="Path 1089" d="M34.055 29.824V0h-5.774v36.295h2.946a9 9 0 0 1 2.828-6.471z"
            fill="#fff">
        </path>
      </g>
    </svg>
    <div class="text">
      <span>
        {{'at '}}
      </span>
       {{' THE SHARD'}}
    </div>
  </a>
</template>

<script setup>

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
  margin-right: 126px;
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
svg:not(:root) {
  overflow: hidden;
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