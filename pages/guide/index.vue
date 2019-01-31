<template>
	<view class="novel-guide">
		<uni-collapse>
			<uni-collapse-item title="正版小说" :open="true">
				<view class="novel-nav-wrap">
					<view class="flex">
						<view class="flex-item" v-for="(item, index) in navlist.original_nav" 
						@click="goTo" 
						:data-name="item.name" 
						:data-url="item.url" 
						:key="index">{{item.name}}</view>
					</view>
				</view>
			</uni-collapse-item>
			<uni-collapse-item title="免费小说" :open="true">
				<view class="novel-nav-wrap">
					<view class="flex">
						<view class="flex-item" v-for="(item, index) in navlist.free_nav" 
						@click="goTo" 
						:data-name="item.name" 
						:data-url="item.url" 
						:key="index">{{item.name}}</view>
					</view>
				</view>
			</uni-collapse-item>
			<!-- <uni-collapse-item title="推荐小说" :open="true">
				手风琴效果2
			</uni-collapse-item> -->
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
		},
		methods:{
			goTo(e){
				let item = e.target.dataset
				//console.log(e, item)
				uni.navigateTo({
					url: '/pages/webview/webview?name=' + item.name + '&url=' + item.url
				});
			}
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
			font-size: 32upx;
			padding: 10upx 0;
		}
		.novel-nav-wrap{
			// padding-left: 40upx;
		}
	}
	
</style>
