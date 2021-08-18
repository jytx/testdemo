<template>
  <view class="index">
    <text>{{ msg }}</text>
    <button @tap="go">tap</button>
  </view>
</template>

<script>
import './index.scss';
import Taro from '@tarojs/taro'

export default {
  data () {
    return {
      msg: 'Hello world!'
    }
  },
  methods: {
    go(){
      Taro.navigateTo({
        url: '/pages/index2/index'
      })
    }
  }
}
</script>
