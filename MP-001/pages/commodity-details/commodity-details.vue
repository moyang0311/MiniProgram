<template>
	<view class="deteli">
		<image src="../../static/icon/详情图.png"></image>
		<span class="text">
			<p>铭瑄（MAXSUN）MS-GeForce RTX3060 iCraft OC 12G DLSS 电竞之心/电脑游戏/光追/直播/设计 显卡</p>
			<p>￥7000</p>
		</span>
		<ul class="list-evaluate">
			<p>评价</p>
			<span class="import">
				<input type="text" value="请输入" style="border: 1rpx solid black;height: 60rpx;width: 386rpx;">
				<button style="width: 160rpx;height: 60rpx;">发送评论</button>
			</span>
			<li v-for="(evaluateData,index) in arrData">
				<span>
					<img :src="evaluateData.img" alt="" style="height: 60rpx;width: 60rpx;border-radius: 100rpx;border: 1rpx solid black;">
					{{evaluateData.name}}
					<span class="none"></span>
					{{evaluateData.date}}
				</span>
				<p>{{evaluateData.text}}</p>
			</li>
		</ul>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				arrData:[
					{
						img:"../../static/icon/headshots.png",
						name:"username",
						date:"2023-7-10",
						text:"用户评论。。。。。。"
					},
					{
						img:"../../static/icon/headshots.png",
						name:"username",
						date:"2023-7-10",
						text:"用户评论。。。。。。"
					},
					{
						img:"../../static/icon/headshots.png",
						name:"username",
						date:"2023-7-10",
						text:"用户评论。。。。。。"
					},
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
	.deteli{
		height: 2000rpx;
		display: flex;
		flex-direction: column;
	}
	image{
		width: 100%;
		height: 744rpx;
	}
	p{
		width: 628rpx;
		height: 146rpx;
		display: flex;
		margin: 0 auto;
	}
	.text{
		width: 750rpx;
		height: 220rpx;
	}
	.text :nth-child(2){
		width: 250rpx;
		font-size: 56rpx;
		display: flex;
		float: right;
	}
	.list-evaluate{
		height: 900rpx;
		width: 670rpx;
		margin: 0 auto;
		border: 1rpx solid black;
		list-style-type: none;
		padding: 20rpx;
	}
	.list-evaluate li{
		margin-top: 10rpx;
	}
	.list-evaluate li span{
		display: flex;
		align-items: center;
		flex-wrap: wrap;
	}
	.list-evaluate p{
		font-size: 40rpx;
	}
	.import{
		display: flex;
		justify-content: space-between;
	}
	.none{
		width: 200rpx;
	}
</style>
