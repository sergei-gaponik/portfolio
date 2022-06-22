<template>
  <div class="a-avatar">
    <div class="a-flex">
      <span>
        <img :height="imgHeight" src="~/assets/img/avatar.png" alt="Sergei Gaponik">
      </span>
      <span class="a-name">
        Sergei Gaponik
      </span>
    </div>
  </div>
</template>

<script>
export default {
  computed: {
    imgHeight(){
      if(this.$device.isDesktop)
        return "100px"
      if(this.$device.isTablet)
        return "80px"
      if(this.$device.isMobile)
        return "60px"
    }
  }
}
</script>


<style scoped>
.a-avatar{
  background-color: var(--c-gray-1);
  border-radius: 100px;
  width: min-content;
  border: 10px solid white;
}
.a-flex{
  display: flex;
  align-items: center;
  gap: var(--gap-s);
}
.a-name{
  white-space: nowrap;
  color: var(--c-blue-1);
  opacity: 80%;
  padding-right: var(--padding);
  font-size: 1.8rem;
  font-weight: 600;
}
</style>