<template>
	<view class="content">
		<view class="logo">
			<img src="../../static/logo.png" alt="">
		</view>
		<view class="search">
			<input type="text">
		</view>
		<view class="user">
			<p>{{user}}</p>
		</view>
	</view>
</template>

<script>
	export default{
		name:'Title',
		data(){
			return{
				title:'hello',
				user:'moyang'
			}
		}
	}
</script>

<style>
	*{
		margin: 0;
		padding: 0;
	}
	.content{
		width: 100%;
		height: 40px;
		border-bottom: 1px solid black;
		background-color: gainsboro;
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: center;
	}
	.logo{
		margin-left: 15px;
	}
	.logo img{
		width: 30px;
		height: 30px;
	}
	.user{
		margin-right: 15px;
	}
	.search input{
		border: 1px solid black;
		border-radius:10px;
		background-color: gray;
	}
</style>