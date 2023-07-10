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
				<uni-swiper-dot :info="info" :current="current" field="content" :mode="mode">
					<swiper class="swiper-box" @change="change">
						<swiper-item v-for="(item ,index) in bunner" :key="index">
							<view class="swiper-item">
								<img class="bmg" :src="item.bmg" alt="">
							</view>
						</swiper-item>
					</swiper>
				</uni-swiper-dot>

			</view>
			<ul class="nav">
				<li v-for="(item,index) in nav" :key="index">
					<img style="width: 48rpx;height: 48rpx;" :src="item.icon">
					<text>{{item.msg}}</text>
				</li>
			</ul>
			<ul class="list">
				<li v-for="(item,index) in things":key="index">
					<img style="width: 160rpx;height: 160rpx;" :src="item.img">
					<text>{{item.name}}</text>
					<text>{{item.price}}</text>
					<navigator url="../deteli/deteli.vue">跳转</navigator>
				</li>
			</ul>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				bunner:[
					{
						bmg:"../../static/icon/index-bunner/001.jpg"
					},
					{
						bmg:"../../static/icon/index-bunner/002.jpg"
					},
					{
						bmg:"../../static/icon/index-bunner/003.jpg"
					},
					{
						bmg:"../../static/icon/index-bunner/004.jpg"
					},
					{
						bmg:"../../static/icon/index-bunner/005.jpg"
					},
				],
				nav:[
					{
						icon:"../../static/icon/index-nav/clothes.png",
						msg:"衣服"
					},{
						icon:"../../static/icon/index-nav/computer.png",
						msg:"电脑"
					},{
						icon:"../../static/icon/index-nav/phone.png",
						msg:"手机"
					},{
						icon:"../../static/icon/index-nav/pen.png",
						msg:"文具"
					},{
						icon:"../../static/icon/index-nav/supermarket.png",
						msg:"超市"
					},{
						icon:"../../static/icon/index-nav/bed.png",
						msg:"家居"
					},{
						icon:"../../static/icon/index-nav/baby.png",
						msg:"母婴"
					},{
						icon:"../../static/icon/index-nav/game.png",
						msg:"游戏"
					},{
						icon:"../../static/icon/index-nav/sport.png",
						msg:"运动"
					},{
						icon:"../../static/icon/index-nav/goodthing.png",
						msg:"好物"
					},
				],
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
				active:true
			}
		},
		methods: {
			change(e) {
				this.current = e.detail.current;
			}
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
		margin: 20rpx 0 ;
		position: relative;
	}
	.bunner .bmg{
		position: absolute;
		left: 0;
		top: 0;
		width: 616rpx;
		height: 228rpx;
		border-radius: 20rpx;
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
