<template>
	<view class="novel-guide">
		<!-- <web-view src="http://m.jingyu.com/index/nboy">360小说</web-view> -->
		<view class="uni-padding-wrap">
			
		</view>
		<uni-collapse accordion="true">
			<uni-collapse-item title="正版小说" :open="true">
				<view class="novel-nav-wrap">
					<view class="flex">
						<view class="flex-item">1</view>
						<view class="flex-item">2</view>
						<view class="flex-item">3</view>
						<view class="flex-item">4</view>
					</view>
				</view>
			</uni-collapse-item>
			<uni-collapse-item title="免费小说" :open="true">
				手风琴效果1
			</uni-collapse-item>
			<uni-collapse-item title="推荐小说" :open="true">
				手风琴效果2
			</uni-collapse-item>
		</uni-collapse>
	</view>
</template>

<script>
	import navlist from "./nav_list"
	import { uniCollapse, uniCollapseItem } from "@dcloudio/uni-ui"
	export default {
		components:{
			uniCollapse,
			uniCollapseItem
		},
		data() {
			return {
				navlist: navlist
			};
		},
		onLoad(){
			console.log(this.navlist)
		}
	}
</script>

<style lang="scss">
	.novel-guide{
		.flex{
			display: flex;
			justify-content:flex-start;
			align-items: center;
			flex-direction: row;
			flex-wrap: wrap;
		}
		.flex-item{
			flex: 0 0 33.3333%;
			text-align: center;
		}
		.novel-nav-wrap{
			// padding-left: 40upx;
		}
	}
	
</style>
