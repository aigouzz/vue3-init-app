<script setup lang="ts">
// import { RouterLink } from "vue-router";
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
        <div class="common">
          <a href="/dist" target="_blank">
            前端架构
            <i class="prev"></i>
            <i class="next"></i>
          </a>
        </div>
        <div class="common">
          <a href="/vue2" target="_blank">
            vue2源码
            <i class="prev"></i>
            <i class="next"></i>
          </a>
        </div>
        <div class="common">
          <a href="/vue3" target="_blank">
            vue3源码
            <i class="prev"></i>
            <i class="next"></i>
          </a>
        </div>
        <div class="common">
          <a href="/react" target="_blank">
            react源码
            <i class="prev"></i>
            <i class="next"></i>
          </a>
        </div>
        <div class="common">
          <a href="/redux" target="_blank">
            redux源码
            <i class="prev"></i>
            <i class="next"></i>
          </a>
        </div>
        <div class="common">
          <a href="/webpack" target="_blank">
            webpack源码
            <i class="prev"></i>
            <i class="next"></i>
          </a>
        </div>
        <div class="common">
          <a href="/algorithm" target="_blank">
            算法-leetcode解析
            <i class="prev"></i>
            <i class="next"></i>
          </a>
        </div>
        <div class="common">
          <a href="/music" target="_blank">
            听音乐
            <i class="prev"></i>
            <i class="next"></i>
          </a>
        </div>
        <div class="common">
          <a href="/shop" target="_blank">
            购物
            <i class="prev"></i>
            <i class="next"></i>
          </a>
        </div>
        <div class="common">
          <a href="/demos" target="_blank">
            查看vue组件
            <i class="prev"></i>
            <i class="next"></i>
          </a>
        </div>
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
nav .common{
  display: inline-block;
  overflow: hidden;
  box-sizing: content-box;
  height: 26px;
}
nav a {
  display: block;
  padding: 0 1rem;
  /* border-left: 1px solid var(--color-border); */
  border: 1px solid transparent;
  height: 24px;
  position: relative;
}
nav a .prev{
  display: block;
  position: absolute;
  top: 50%;
  left: 50%;
  transform-origin: 0 0;
  background: goldenrod;
  animation: rotating 3s linear infinite;
  width: 100%;
  height: 48px;
  z-index: -2;
}
nav a .next{
  background: var(--vt-c-white);
  z-index: -1;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 24px;
}
@keyframes rotating{
  from{
    transform: rotate(0);
  }
  to{
    transform: rotate(360deg);
  }
}

nav a:first-of-type {
  /* border: 0; */
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
