<template>
  <div class="father-wrap">
    <div class="father-title">这是父元素title</div>
    <Child>
      <template v-slot:title>
        <h4>这是子元素title</h4>
      </template>
      <template v-slot:content>
        <span>这是子元素的内容</span>
      </template>
    </Child>
  </div>
</template>
<script lang="ts">
import Child from "../components/common/ChildType.vue";
export default {
  components: {
    Child,
  },
};
</script>
