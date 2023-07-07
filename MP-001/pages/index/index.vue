<template>
	<view>
		<view class="top">
			<view class="search">
				<input type="text" placeholder="手机">
				<button>搜索</button>
			</view>
		</view>
		<view class="content">
			<view class="bunner">
				
			</view>
				<ul class="nav">
					<li>
						<img style="width: 48rpx;height: 48rpx;" src="../../static/icon/index-nav/clothes.png">
						<text>衣服</text>
					</li>
					<li>
						<img style="width: 48rpx;height: 48rpx;" src="../../static/icon/index-nav/computer.png">
						<text>电脑</text>
					</li>
					<li>
						<img style="width: 48rpx;height: 48rpx;" src="../../static/icon/index-nav/phone.png">
						<text>手机</text>
					</li>
					<li>
						<img style="width: 48rpx;height: 48rpx;" src="../../static/icon/index-nav/pen.png">
						<text>文具</text>
					</li>
					<li>
						<img style="width: 48rpx;height: 48rpx;" src="../../static/icon/index-nav/supermarket.png">
						<text>超市</text>
					</li>
					<li>
						<img style="width: 48rpx;height: 48rpx;" src="../../static/icon/index-nav/bed.png">
						<text>家居</text>
					</li>
					<li>
						<img style="width: 48rpx;height: 48rpx;" src="../../static/icon/index-nav/baby.png">
						<text>母婴</text>
					</li>
					<li>
						<img style="width: 48rpx;height: 48rpx;" src="../../static/icon/index-nav/game.png">
						<text>游戏</text>
					</li>
					<li>
						<img style="width: 48rpx;height: 48rpx;" src="../../static/icon/index-nav/sport.png">
						<text>运动</text>
					</li>
					<li>
						<img style="width: 48rpx;height: 48rpx;" src="../../static/icon/index-nav/goodthing.png">
						<text>好物</text>
					</li>
				</ul>
				<ul class="list">
					<li>
						<img style="width: 160rpx;height: 160rpx;" src="../../static/icon/index-list/computer.jpg" alt="">
						<text>笔记本电脑</text>
						<text>￥3000</text>
					</li>
					<li>
						<img style="width: 160rpx;height: 160rpx;" src="../../static/icon/index-list/computer.jpg" alt="">
						<text>笔记本电脑</text>
						<text>￥3000</text>
					</li><li>
						<img style="width: 160rpx;height: 160rpx;" src="../../static/icon/index-list/computer.jpg" alt="">
						<text>笔记本电脑</text>
						<text>￥3000</text>
					</li><li>
						<img style="width: 160rpx;height: 160rpx;" src="../../static/icon/index-list/computer.jpg" alt="">
						<text>笔记本电脑</text>
						<text>￥3000</text>
					</li><li>
						<img style="width: 160rpx;height: 160rpx;" src="../../static/icon/index-list/computer.jpg" alt="">
						<text>笔记本电脑</text>
						<text>￥3000</text>
					</li><li>
						<img style="width: 160rpx;height: 160rpx;" src="../../static/icon/index-list/computer.jpg" alt="">
						<text>笔记本电脑</text>
						<text>￥3000</text>
					</li><li>
						<img style="width: 160rpx;height: 160rpx;" src="../../static/icon/index-list/computer.jpg" alt="">
						<text>笔记本电脑</text>
						<text>￥3000</text>
					</li><li>
						<img style="width: 160rpx;height: 160rpx;" src="../../static/icon/index-list/computer.jpg" alt="">
						<text>笔记本电脑</text>
						<text>￥3000</text>
					</li><li>
						<img style="width: 160rpx;height: 160rpx;" src="../../static/icon/index-list/computer.jpg" alt="">
						<text>笔记本电脑</text>
						<text>￥3000</text>
					</li><li>
						<img style="width: 160rpx;height: 160rpx;" src="../../static/icon/index-list/computer.jpg" alt="">
						<text>笔记本电脑</text>
						<text>￥3000</text>
					</li><li>
						<img style="width: 160rpx;height: 160rpx;" src="../../static/icon/index-list/computer.jpg" alt="">
						<text>笔记本电脑</text>
						<text>￥3000</text>
					</li><li>
						<img style="width: 160rpx;height: 160rpx;" src="../../static/icon/index-list/computer.jpg" alt="">
						<text>笔记本电脑</text>
						<text>￥3000</text>
					</li>
				</ul>
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
		justify-content: center;
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
	.bunner{
		width: 616rpx;
		height: 228rpx;
		background-color: #000;
		border-radius: 40rpx;
		margin: 20rpx 0 ;
	}
	.nav{
		width: 600rpx;
		height: 212rpx;
		/* background-color: #bbb; */
		display: flex;
		flex-wrap: wrap;
		align-content: ;
		align-items: center;
		justify-content: space-around;
	}
	.nav li{
		width: 120rpx;
		height: 88rpx;
		font-size: 28rpx;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	.list{
		width: 600rpx;
		height: auto;
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		align-content: space-around;
		justify-content: space-around;
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
