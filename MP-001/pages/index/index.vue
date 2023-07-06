<template>
	<view>
		<view class="search">
			<input type="text" placeholder="手机">
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
	page{
		background-color: #75F9FD;
	}
	.search{
		margin-top: 20rpx;
		margin: 0 auto;
		width: 80%;
		border: 1rpx solid #bbb;
		height: 60rpx;
		border-radius: 20px;
		background-color: #fff;
	}
	.search input{
		margin-left: 20rpx;
		line-height: 60rpx;
	}
</style>
