<script setup lang="ts">
defineProps<{
  msg: string;
}>();
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      欢迎关注我的博客，详情请阅读
      <br />
      <a href="/dist" target="_blank" rel="noopener">前端介绍</a> +
      <a href="/music" target="_blank" rel="noopener">网易云音乐项目</a> +
      <a href="/shop" target="_blank" rel="noopener">商城项目</a>
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
