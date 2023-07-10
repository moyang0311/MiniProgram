<template>
	<view>
		<view class="top">
			<view class="search">
				<input type="text" placeholder="手机">
				<navigator url="../search/search">
					<button>搜索</button>
				</navigator>
			</view>
		</view>
		<view class="content">
			<ul class="list">
				<li v-for="(item,index) in things":key="index">
					<img style="width: 160rpx;height: 160rpx;" :src="item.img">
					<text>{{item.name}}</text>
					<text>{{item.price}}</text>
				</li>
			</ul>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				things:[
					{
						img:'../../static/icon/index-list/computer.jpg',
						name:'电脑',
						price:"￥3000"
					},{
						img:'../../static/icon/index-list/computer.jpg',
						name:'电脑',
						price:"￥3000"
					},{
						img:'../../static/icon/index-list/computer.jpg',
						name:'电脑',
						price:"￥3000"
					},{
						img:'../../static/icon/index-list/computer.jpg',
						name:'电脑',
						price:"￥3000"
					},{
						img:'../../static/icon/index-list/computer.jpg',
						name:'电脑',
						price:"￥3000"
					},{
						img:'../../static/icon/index-list/computer.jpg',
						name:'电脑',
						price:"￥3000"
					},{
						img:'../../static/icon/index-list/computer.jpg',
						name:'电脑',
						price:"￥3000"
					},{
						img:'../../static/icon/index-list/computer.jpg',
						name:'电脑',
						price:"￥3000"
					},{
						img:'../../static/icon/index-list/computer.jpg',
						name:'电脑',
						price:"￥3000"
					},{
						img:'../../static/icon/index-list/computer.jpg',
						name:'电脑',
						price:"￥3000"
					}
				],
			}
		},
		methods: {
			
		}
	}
</script>

<style>
	page{
		background-color: aqua;
	}
	.top{
		width: 100%;
		height: 180rpx;
		/* background-color: #000; */
		display: flex;
		justify-content: center;
		align-items: center;
	}
	.search{
		width: 676rpx;
		height: 88rpx;
		background-color: #fff;
		border: 1px solid #bbb;
		border-radius: 44rpx;
		display: flex;
		justify-content: space-between;
		align-items: center;
	}
	.search input{
		height: 88rpx;
		/* background-color: #000; */
		margin-left: 50rpx;
	}
	.search button{
		width: 190rpx;
		height: 88rpx;
		background-color: #75fdc4;
		border-radius: 0rpx 44rpx 44rpx 0 ;
		margin-right: 0;
		text-align: center;
		line-height: 88rpx;
	}
	.content{
		width: 100%;
		height: 100%;
		background-color: #fff;
		border-radius: 64rpx 64rpx 0 0 ;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: space-around;
	}
	.list{
		width: 600rpx;
		height: auto;
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		align-content: space-around;
		justify-content: space-around;
		margin-top: 40rpx;
	}
	.list li{
		width: 258rpx;
		height: 272rpx;
		border: 1rpx solid #bbb;
		border-radius: 33rpx;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		margin-bottom: 20rpx;
	}
	.list li text:nth-child(3){
		color: #0094FF;	
	}
</style>
