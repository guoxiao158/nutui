<template>
  <view class="test">
    <text>{{ msg }}</text>
    <text>{{ title }}</text>
    <slot></slot>
  </view>
</template>

<script>
import { ref } from 'vue';
export default {
  props: {
    title: String
  },
  setup() {
    const msg = ref('test');
    return {
      msg
    };
  }
};
</script>

<style>
.test {
  border: 1px solid red;
}
</style>
