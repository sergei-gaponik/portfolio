<template>
  <div class="a-reference">
    <div class="a-title">{{ reference.title }}</div>
    <div>
      <ul class="a-ul">
        <li class="a-li" v-for="(item, i) in reference.content" :key="i">{{ item }}</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  props: ["reference"]
}
</script>

<style scoped>
.a-reference{
  background-color: var(--c-purple-3);
  border-radius: var(--border-radius);
  padding: 3rem;
}
.a-title{
  font-size: 1.8rem;
  color: var(--c-purple-2);
  font-weight: 500;
}
.a-ul{
  font-size: 1.3rem;
  font-weight: 300;
  color: var(--c-gray-2);
}
.a-li:not(:last-child) {
    margin-bottom: 0.8rem;
}
</style>