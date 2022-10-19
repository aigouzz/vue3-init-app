<template>
  <div class="index__404">
    <div class="index__404-title">您到了一片知识的荒漠</div>
    <RouterLink to="/">回到首页</RouterLink>
  </div>
</template>
<script setup lang="ts">
import { RouterLink } from 'vue-router';

</script>
<style scoped lang="less">
.index__404{
    width: 1360px;
    margin: 0 auto;
    .index__404-title{
        line-height: 38px;
    }
    a{
        display: block;
        width: 140px;
        line-height: 38px;
    }
}
</style>