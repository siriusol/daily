<template>
    <view>
        <DailyHeader />
        <swiper class="swiper" :indicator-dots="indicatorDots" :indicator-active-color="activeColor" :autoplay="true">
            <swiper-item v-for="(item, index) in banners" :key="index">
                <image :src="item" mode="widthFix"></image>
            </swiper-item>
        </swiper>
    </view>
</template>

<script>
    import DailyHeader from '../../components/DailyHeader.vue'
	export default {
		data() {
			return {
                indicatorDots: true,
                activeColor: "#ffc81f",
                banners: [
                    "https://img.36krcdn.com/hsossms/20230127/v2_0e1500e5181444c899355f6e0ee88444_oswg190068oswg1440oswg600_img_jpg",
                    "https://img.36krcdn.com/hsossms/20230127/v2_d5b5c81f60b949f8819b531742bf69ce_oswg1673882oswg1440oswg600_img_png",
                    "https://img.36krcdn.com/hsossms/20230119/v2_7c2f01ec78ad48208c551a2f6246b906_oswg1113850oswg1440oswg600_img_png"
                ]
			}
		},
        components: {
            DailyHeader
        },
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss">
    .swiper {
        image {
            // height: calc(100vw * 600 / 1440);
            width: 100vw;
        }
    }
</style>
