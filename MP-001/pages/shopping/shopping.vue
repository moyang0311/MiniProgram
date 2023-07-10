<template>
	<view>
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
		background-color: #000;
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
</style>
