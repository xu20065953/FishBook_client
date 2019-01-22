<template>
	<view class="content">
        <swiper autoplay="true" indicator-dots="true" circular="true" style="height: 400upx;">
            <swiper-item v-for="(img,key) in imgUrls" :key="key">
                <image :src="img" style="height: 400upx;" />
            </swiper-item>
        </swiper>
		
		<view class="">
			dsad
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				imgUrls: [
				    'https://img-cdn-qiniu.dcloud.net.cn/uniapp/images/shuijiao.jpg',
				    'https://img-cdn-qiniu.dcloud.net.cn/uniapp/images/muwu.jpg',
				    'https://img-cdn-qiniu.dcloud.net.cn/uniapp/images/cbd.jpg'
				]
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.content {
		text-align: center;
		height: 400upx;
	}
    .logo{
        height: 200upx;
        width: 200upx;
        margin-top: 200upx;
    }
	.title {
		font-size: 36upx;
		color: #8f8f94;
	}
	.swiper{
		width: 750upx;
		height: 346upx;
	}
	image {
	    width: 100%;
	}
</style>
