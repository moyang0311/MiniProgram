<template>
	<view class="content">
		<text class="totality">全部 0</text>
		<ul>
			<li v-for="(shopData, index) in arrData">
				<!-- 购物车盒子 -->
				<view class="shopBox">
					<!-- 商店名选择 -->
					<label class="storechoes">
						<radio value="选择" :checked = "shopData.status"/>
							{{shopData.shopName}}
					</label>
					<view class="deteli">
						<label class="radio">
							<radio value="" /><text></text>
						</label>
						<!-- 图片 -->
						<view class="img">
							<img :src="shopData.imgs" width="100%;" height="auto"/>			
						</view>
									<!-- 商品详情 -->
						<view class="commodity">
							<span>商品名称：{{shopData.name}}</span><br>
							<span>价格:￥{{shopData.price}}</span><br>
							<span class="count" @click="shopData.count++">+ &nbsp;&nbsp;</span>
							<span class="count">数量：{{shopData.count}}
							</span><span class="count" @click="shopData.count--">&nbsp;&nbsp;-</span><br>
						</view>	
					</view>
							
				</view>
			</li>
			
		</ul>
		<view class="footer">
			<label class="radio">
				<radio value="all" /><text>全选</text>
			</label>
			<view class="total_price">
				<text>合计:</text>
				<text>￥0.00</text>
			</view>
			<view class="pay">
				<text>去结算</text>
			</view>
		</view>
	</view>
	
</template>

<script>
	export default {
		data() {
			return {
				arrData:[
					{
					name:'电脑',
					status:true,
					imgs:'https://gd4.alicdn.com/imgextra/i1/84767494/O1CN01LnKAJf25EIyTJEqn6_!!84767494.jpg',
					shopName:'华硕商城',
					price:3888,
					count:3,
					
				},
				{
					name:'电脑',
					status:false,
					imgs:'https://gd4.alicdn.com/imgextra/i1/84767494/O1CN01LnKAJf25EIyTJEqn6_!!84767494.jpg',
					shopName:'华为商城',
					price:3888,
					count:3,
				},
				{
					name:'电脑',
					status:true,
					imgs:'https://gd4.alicdn.com/imgextra/i1/84767494/O1CN01LnKAJf25EIyTJEqn6_!!84767494.jpg',
					shopName:'华硕商城',
					price:3888,
					count:3,
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
		background-color: #d6d6d6;
	}
	.content{
		width: 100%;
		height: 100%;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
	.totality{
		color: #75F9FD;
		font-size: 36rpx;
	}
	ul{
		width: 100%;
		height: auto;
		list-style-type: none;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
	ul li{
		width: 660rpx;
		height: 340rpx;
		background-color: #fff;
		border: 1rpx solid #bbb;
		border-radius: 40rpx;
		margin-top: 50rpx;
	}
	.storechoes{
		height: 100rpx;
		width: 100%;
		/* background-color: red; */
		display: block;
		line-height: 100rpx;
	}
	.img{
		width: 212rpx;
		height: 212rpx;
		/* background-color: #000; */
	}
	.img img{
		width: 100%;
		height: 100%;
		border-radius: 40rpx;
	}
	.deteli{
		width: 100%;
		height: auto;
		display: flex;
		justify-content: space-around;
		align-items: center;
	}
	.count{
		margin-left: 40rpx;
	}
	.footer{
		width: 100%;
		height: 112rpx;
		background-color: #fff;
		border: 1rpx solid #bbb;
		position: sticky;
		bottom: 0;
		display: flex;
		justify-content: space-around;
		align-items: center;	
	}
	.total_price{
		font-size: 36rpx;
	}
	.pay{
		width: 162rpx;
		height: 66rpx;
		border: 1px solid #bbb;
		background-color: #75F9FD;
		border-radius: 33rpx;
		display: flex;
		align-items: center;
		justify-content: center;
	}
</style>
