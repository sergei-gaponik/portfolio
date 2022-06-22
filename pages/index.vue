<template>
<div style="overflow-x: hidden !important;">
  <hero />
  <div :style="{ marginBottom: heroMarginBottom }"></div>
  <bio />
  <references style="margin-bottom:6rem" />
  <Footer />
</div>
</template>

<script>
export default {
  computed: {
    heroMarginBottom(){
      if(this.$device.isDesktop)
        return "200px"
      if(this.$device.isTablet)
        return "180px"
      if(this.$device.isMobile)
        return "200px"
    }
  }
}
</script>
