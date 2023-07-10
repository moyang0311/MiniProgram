<template>
	<view class="userbox">
		<view class="headshots">
			<img src="../../static/icon/headshots.png">
			<image src="../../static/icon/headshots.png"></image>
			<p>
				username
			</p>
		</view>
		<view class="list">
			<ul>
				<li>
					<span>
						<img src="../../static/icon/payment.png">
						<p>待付款</p>
					</span>
					<span>
						<img src="../../static/icon/expressage.png">
						<p>待收货</p>
					</span>
					<span>
						<img src="../../static/icon/evaluate.png">
						<p>评价</p>
					</span>
				</li>
				<li v-for="(userData,index) in listData">
					<img :src="userData.imgs" alt="" style="height: 70rpx;width: 70rpx;">
					<span class="list-text">{{userData.text}}</span>
				</li>
			</ul>
		</view>
	</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				listData:[
					{
						imgs:'../../static/icon/personage.png',
						text:'个人信息',
					},
					{
						imgs:'../../static/icon/record.png',
						text:'消费记录',
					},
					{
						imgs:'../../static/icon/setting.png',
						text:'设置',
					}
				]
			}
		},
		methods: {
			
		}
	}
</script>

<style>
	*{
		margin: 0;
		padding: 0;
	}
	page{
		background-color:aquamarine;
	}
	.userbox{
		width: 100%;
		display: flex;
		flex-direction: column;
	}
	.headshots{
		margin: 0 auto;
		padding-top: 55rpx;
		width: 250rpx;
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
		width: 520rpx;
		background-color: white;
		border-top-left-radius: 50rpx;
		border-top-right-radius: 50rpx;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	.list ul {
		height: 710rpx;
		width: 440rpx;
		list-style-type: none;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	.list ul li{
		height: 150rpx;
		width: 440rpx;
		display: inline-flex;
		margin-top: 40rpx;
		justify-content: space-between;
	}
	.list ul li span{
		text-align: center;
	}
	.list ul li span image{
		height: 70rpx;
		width: 70rpx;
	}
	.list-text{
		width: 140rpx;
		height: 70rpx;
		display: flex;
		align-items: center;
		margin-right: auto;
	}
</style>
