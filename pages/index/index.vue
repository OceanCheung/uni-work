<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<text class="title">{{title}}</text>
		</view>
		<uni-rate value="rate"></uni-rate>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: '首页',
				rate:3
			}
		},
		methods: {
		
		},
		onLoad() {
			// #ifdef H5 || APP-PLUS
			console.log(111);
			// #endif
			console.log("index--请求数据。。。");
		},
		onShow() {
			console.log("index--页面显示。。。");
		},
		onReady() {
			console.log("index--页面加载完成。。。");
			uni.navigateTo({
			    url: '../list/index?id=1&name=zhangsan'
			});
		}
		
	}
</script>

<style lang="scss">
	@import "./index.scss";
	/* #ifdef APP-PLUS || H5 */
		
	/* #endif */
</style>
