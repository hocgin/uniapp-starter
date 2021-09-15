<template>
  <view class="content">
    <image class="logo" src="../../static/logo.png"></image>
    <view>
      <text class="title">{{ title }}</text>
      <text class="title">Hello Word</text>
      <u-button type="primary">主要按钮</u-button>
      <u-rate :count="count" v-model="value"></u-rate>
    </view>
  </view>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  data() {
    return {
      title: 'Hello',
      count: 4,
      value: 2
    }
  },
  onLoad() {

  },
  methods: {}
});
</script>

<style type="text/scss" lang="scss">
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.logo {
  height: "200rpx";
  width: "200rpx";
  margin: "200rpx" auto "50rpx" auto;
}

.text-area {
  display: flex;
  justify-content: center;
}

.title {
  font-size: "36rpx";
  color: #8f8f94;
}
</style>
