<template>
  <view class="box">
    <!-- 自定义组件 -->
    <search />

    <!-- 轮播图 -->
    <view class="banner">
      <swiper
        indicator-dots
        indicator-color="rgba(255,255,255,.6)"
        indicator-active-color="#fff"
        autoplay
        circular
        interval="3000"
      >
        <swiper-item>
          <navigator url>
            <image src="/static/uploads/banner1.png" />
          </navigator>
        </swiper-item>
        <swiper-item>
          <navigator url>
            <image src="/static/uploads/banner2.png" />
          </navigator>
        </swiper-item>
        <swiper-item>
          <navigator url>
            <image src="/static/uploads/banner3.png" />
          </navigator>
        </swiper-item>
      </swiper>
    </view>

    <!-- 导航栏 -->
    <view class="naver">
      <view>
        <navigator url>
          <image src="../../static/uploads/icon_index_nav_4@2x.png" />
        </navigator>
      </view>
      <view>
        <navigator url>
          <image src="../../static/uploads/icon_index_nav_3@2x.png" />
        </navigator>
      </view>
      <view>
        <navigator url>
          <image src="../../static/uploads/icon_index_nav_2@2x.png" />
        </navigator>
      </view>
      <view>
        <navigator url>
          <image src="../../static/uploads/icon_index_nav_1@2x.png" />
        </navigator>
      </view>
    </view>

    <!-- 商品展示(楼层) -->
    <view class="fools">
      <view class="fool">
        <!-- 标题 -->
        <view class="title">
          <image src="/static/uploads/pic_floor01_title.png" />
        </view>
        <!-- 内容 -->
        <view class="item">
          <navigator url>
            <image src="/static/uploads/pic_floor01_1@2x.png" />
          </navigator>
          <navigator url>
            <image src="/static/uploads/pic_floor01_2@2x.png" />
          </navigator>
          <navigator url>
            <image src="/static/uploads/pic_floor01_3@2x.png" />
          </navigator>
          <navigator url>
            <image src="/static/uploads/pic_floor01_4@2x.png" />
          </navigator>
          <navigator url>
            <image src="/static/uploads/pic_floor01_5@2x.png" />
          </navigator>
        </view>
      </view>
      <view class="fool">
        <!-- 标题 -->
        <view class="title">
          <image src="/static/uploads/pic_floor02_title.png" />
        </view>
        <!-- 内容 -->
        <view class="item">
          <navigator url>
            <image src="/static/uploads/pic_floor02_1@2x.png" />
          </navigator>
          <navigator url>
            <image src="/static/uploads/pic_floor02_2@2x.png" />
          </navigator>
          <navigator url>
            <image src="/static/uploads/pic_floor02_3@2x.png" />
          </navigator>
          <navigator url>
            <image src="/static/uploads/pic_floor02_4@2x.png" />
          </navigator>
          <navigator url>
            <image src="/static/uploads/pic_floor02_5@2x.png" />
          </navigator>
        </view>
      </view>
      <view class="fool">
        <!-- 标题 -->
        <view class="title">
          <image src="/static/uploads/pic_floor03_title.png" />
        </view>
        <!-- 内容 -->
        <view class="item">
          <navigator url>
            <image src="/static/uploads/pic_floor03_1@2x.png" />
          </navigator>
          <navigator url>
            <image src="/static/uploads/pic_floor03_2@2x.png" />
          </navigator>
          <navigator url>
            <image src="/static/uploads/pic_floor03_3@2x.png" />
          </navigator>
          <navigator url>
            <image src="/static/uploads/pic_floor03_4@2x.png" />
          </navigator>
          <navigator url>
            <image src="/static/uploads/pic_floor03_5@2x.png" />
          </navigator>
        </view>
      </view>
    </view>
  </view>
</template> 

<script>
// 导入自定义的组件
import search from "@/components/search.vue";

export default {
  data() {
    return {};
  },

  // 注册组件
  components: {
    search
  },

  onLoad() {},

  methods: {}
};
</script>

<style lang="less">

// 轮播图
.banner {
  swiper {
    height: 340rpx;
  }
  image {
    width: 750rpx;
    height: 340rpx;
  }
}
// 导航
.naver {
  height: 192rpx;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0rpx 30rpx;
  navigator {
    width: 128rpx;
    height: 140rpx;
  }
}

// 楼层

.fool {
  // 标题
  .title {
    width: 750rpx;
    height: 60rpx;
    background-color: #f4f4f4;
    padding-top: 30rpx;
    padding-left: 10rpx;
  }
  .item {
    overflow: hidden;
    padding: 20rpx 16rpx;
    navigator {
      float: left;
      margin-left: 10rpx;
    }
    navigator:first-child {
      width: 232rpx;
      height: 386rpx;
      margin-left: 0rpx;
    }
    navigator:nth-child(3),
    navigator:nth-child(4) {
      width: 193rpx;
      height: 188rpx;
    }
    navigator:nth-child(2),
    navigator:nth-child(5) {
      width: 273rpx;
      height: 188rpx;
    }
    navigator:nth-last-child(-n + 2) {
      margin-top: 10rpx;
    }
  }
  &:first-child {
    .item {
      navigator {
        width: 233rpx;
        height: 188rpx;
      }
      navigator:first-child {
        width: 232rpx;
        height: 386rpx;
      }
    }
  }
}
</style>
