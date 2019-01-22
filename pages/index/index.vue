<template>
	<view class="content">
        <swiper class="swiper" :indicator-dots="true" :autoplay="false" :interval="3000" :duration="1000">
        	<swiper-item>
        		<view class="swiper-item">
					<image style="width: 100%;" src="//edu-image.nosdn.127.net/337d29d51ba944b99169dbad13bb9639.jpg?imageView&crop=0_0_1242_573&quality=100&thumbnail=750y346&type=webp" mode="scaleToFill"></image>
				</view>
        	</swiper-item>
        	<swiper-item>
        		<view class="swiper-item">
					<image style="width: 100%;" src="//edu-image.nosdn.127.net/e1879b3c3b0a4702b66b0e10538d79ad.png?imageView&crop=0_0_1242_573&quality=100&thumbnail=750y346&type=webp" mode="scaleToFill"></image>
				</view>
        	</swiper-item>
        	<swiper-item>
        		<view class="swiper-item">
					<image style="width: 100%;" src="//edu-image.nosdn.127.net/a33fc91fd60542c597b89b764cbc4bbd.jpg?imageView&crop=0_0_1242_573&quality=100&thumbnail=750y346&type=webp" mode="scaleToFill"></image>
				</view>
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
</style>
