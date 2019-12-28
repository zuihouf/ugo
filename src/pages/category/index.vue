<template>
  <view>
      <!-- 自定义组件 -->
    <search />
  </view>
</template>

<script>
// 引入自定义组件
import search from "@/components/search";

export default {
  // 注册组件
  components: {
    search
  }
};
</script>

<style lang="less">
</style>
