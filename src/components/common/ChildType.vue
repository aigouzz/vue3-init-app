<template>
  <div class="index__child">
    <slot name="title"></slot>
    <slot name="content"></slot>
  </div>
</template>
<script setup lang="ts">
import { getCurrentInstance } from 'vue'

interface Props {
  name: string,
  rent?: () => null
}
let props = withDefaults(defineProps<Props>(), {
  name: '',
  rent: () => {
    return null
  }
});
const instance = getCurrentInstance();

console.log()

</script>
<style lang="less" scoped>
.index__child {
  width: 100%;
}
</style>
