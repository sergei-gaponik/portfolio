<template>
  <div class="a-bg">
    <div class="container">
      <h2 class="a-title">Kontakt</h2>
      <div class="a-content flex-v-s">
        <div>Sergei Gaponik</div>
        <a class="a-mail" href="mailto:info@gaponik.com">info@gaponik.com</a>
        <a class="a-link" href="https://www.linkedin.com/in/sergei-gaponik/">LinkedIn</a>
      </div>
    </div>
  </div>
</template>

<style scoped>
.a-bg{
  background-color: var(--c-blue-1);
}
.a-title{
  color: white;
}
.a-content{
  font-size: 1.3rem;
  color: white;
  font-weight: 300;
  padding-bottom: 3rem;
}
.a-mail{
  text-decoration: none;
  font-weight: 600;
  color: white;
}
.a-link{
  text-decoration: underline;
  color: white;
}
</style>