<template>
  <view class="index">
    <text>{{ msg }}</text>
    <nut-button type="primary" desc="主要按钮">主要按钮</nut-button>
    <nut-button type="info">信息按钮</nut-button>
    <nut-button type="default">默认按钮</nut-button>
    <nut-button type="danger">危险按钮</nut-button>
    <nut-button type="warning">警告按钮</nut-button>
    <nut-button type="success">成功按钮</nut-button>
    <test>solt</test>
  </view>
</template>

<script>
import { ref } from 'vue';
import './index.scss';
// import Button from '../../../../../../packages/__VUE/button/index.taro.vue';
import Button from '../button/index.taro.vue';
// import test from '../../../../test.vue';
import test from './test.vue';
export default {
  components: {
    'nut-button': Button,
    test
  },
  setup() {
    const msg = ref('Hello world,Test NutUI');
    return {
      msg
    };
  }
};
</script>
