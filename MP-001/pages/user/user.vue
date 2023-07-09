<template>
	<view class="userbox">
		<view class="headshots">
			<image src="../../static/icon/headshots.png"></image>
			<p>
				username
			</p>
		</view>
		<view class="list">
			
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style>
	.userbox{
		height: 100%;
		width: 100%;
		background-color: aquamarine;
		display: flex;
		flex-direction: column;
	}
	.headshots{
		margin: 0 auto;
		padding-top: 55rpx;
		width: 250rpx;
		/* border: 1rpx solid black; */
		text-align: center;
	}
	.headshots image{
		margin: 0 auto;
		height: 200rpx;
		width: 200rpx;
		border: 1rpx solid black;
		border-radius: 100rpx;
	}
	.list{
		margin: 0 auto;
		height: 840rpx;
		width: 520rpx;
		background-color: white;
		border-top-left-radius: 50rpx;
		border-top-right-radius: 50rpx;
	}
</style>
