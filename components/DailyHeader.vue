<template>
    <view class="header">
        <image src="@/static/images/icon.png" mode="widthFix"></image>
        <text class="iconfont icon-search"></text>
    </view>
</template>

<script>
    export default {
        name:"DailyHeader",
        data() {
            return {
                
            };
        }
    }
</script>

<style lang="scss">
    @import url('@/iconfont/iconfont.css');
	.header {
        background: #000;
        height: 88rpx;
        padding: 6rpx 30rpx;
        image {
            width: 5%;
        }
        display: flex;
        justify-content: space-between;
        align-items: center;
        text {
            color: #fff;
        }
    }
</style>