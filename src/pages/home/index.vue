<template>
  <view class="home">
    <view class="title">111</view>
    <uni-badge
      :text="100"
      type="default"
      size="normal"
    />
    <u-calendar :show="show"  @confirm="confirm"></u-calendar>
		<u-button @click="show = true">打开</u-button>
  </view>
</template>

<script>
export default {
  name: "home",
  components: {},
  props: {},
  data() {
    return {
      show: false
    }
  },
  computed: {},
  methods: {
    confirm(val) {
      console.log(val)
      this.show = false
    }
  },
  watch: {},

  // 页面周期函数--监听页面加载
  onLoad() {},
  // 页面周期函数--监听页面初次渲染完成
  onReady() {},
  // 页面周期函数--监听页面显示(not-nvue)
  onShow() {},
  // 页面周期函数--监听页面隐藏
  onHide() {},
  // 页面周期函数--监听页面卸载
  onUnload() {},
  // 页面处理函数--监听用户下拉动作
  // onPullDownRefresh() { uni.stopPullDownRefresh(); },
  // 页面处理函数--监听用户上拉触底
  // onReachBottom() {},
  // 页面处理函数--监听页面滚动(not-nvue)
  // onPageScroll(event) {},
  // 页面处理函数--用户点击右上角分享
  // onShareAppMessage(options) {},
} 
</script>

<style scoped lang="scss">
  .home{
    width: 100rpx;
    .title{
      color: $colorem01;
    }
  }
</style>