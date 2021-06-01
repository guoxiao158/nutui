<template>
  <view class="test">
    <text>{{ msg }}</text>
    <slot></slot>
  </view>
</template>

<script>
import { ref } from 'vue';
export default {
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
