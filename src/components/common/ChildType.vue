<template>
  <div class="child">
    <slot name="title"></slot>
    <slot name="content"></slot>
  </div>
</template>
<script lang="ts">
export default {
  setup() {},
};
</script>
<style lang="less" scoped>
.child {
  width: 100%;
}
</style>
