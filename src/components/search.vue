<template>
  <!-- 搜索 -->
  <!-- 输入框 -->
  <view class="search">
    <view class="input-box">
      <input type="text" />
    </view>
    <!-- 搜索内容 -->
    <view class="content"></view>
  </view>
</template>

<script>
export default {};
</script>

<style lang="less">
// 搜索
.search {
  .input-box {
    background-color: #ea4451;
    padding: 20rpx 16rpx;
    input {
      width: 100%;
      height: 60rpx;
      border-radius: 6rpx;
      background-color: #fff;
    }
  }
}
</style>