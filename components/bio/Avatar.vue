<template>
  <div class="a-avatar">
    <div class="a-flex">
      <span>
        <img class="a-img" src="~/assets/img/avatar.png" alt="Sergei Gaponik">
      </span>
      <span class="a-name">
        Sergei Gaponik
      </span>
    </div>
  </div>
</template>

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
  color: #262B32bb;
  padding-right: var(--padding);
  font-size: 1.8rem;
  font-weight: 600;
}

.a-img{
  height: 100px;
}

@media only screen and (max-width: 900px) {
  .a-img{
    height: 80px;
  }
}

@media only screen and (max-width: 600px) {
  .a-img{
    height: 60px;
  }
}
</style>