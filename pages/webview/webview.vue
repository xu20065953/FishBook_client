<template>
	<view>
		<web-view :src="url"></web-view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				url: "",
				name: ""
			};
		},
		onLoad(option){
			this.url = option.url;
			this.name = option.name;
			uni.setNavigationBarTitle({
				title: this.name
			});
		}
	}
</script>

<style lang="scss">

</style>
