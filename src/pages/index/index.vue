<template>
  <view class="index">
    <text>{{ msg }}</text>
  </view>
   <nut-button type="primary" size="large">{{ msg }}</nut-button>

  <view>
    <view class=" .footer">Copyright © 学院路共同体</view>
  </view>
</template>

<script>
import { ref } from 'vue'
import './index.scss'
import { Button as NutButton } from "@nutui/nutui-taro";
// 引入所有组件的样式文件
import "@nutui/nutui-taro/dist/style.css";

export default {
  setup () {
    const msg = ref('你好')
    return {
      msg
    }
  },
  components: {
    NutButton 
  }
}
</script>
