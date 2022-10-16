<script setup lang="ts">
import { RouterLink } from "vue-router";
import LeftMessage from "../components/LeftMessage.vue";
import TheWelcome from "../components/TheWelcome.vue";
</script>

<template>
  <header>
    <img
      alt="个人博客"
      class="logo"
      src="@/assets/logo.svg"
      width="125"
      height="125"
    />

    <div class="wrapper">
      <LeftMessage msg="个人博客" />

      <nav>
        <a href="/dist" target="_blank">前端架构</a>
        <a href="/music" target="_blank">听音乐</a>
        <a href="/shop" target="_blank">购物</a>
        <a href="/demos" target="_blank">查看vue组件</a>
      </nav>
    </div>
  </header>
  <main>
    <TheWelcome></TheWelcome>
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
