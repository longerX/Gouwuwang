<template>
	<view class="container">
		<!-- 搜索框 -->
		<view class="search">
			<input type="text" placeholder="请输入搜索内容" style="width:80%;display:inline-block;height:30px;font-size:18px;"/>
			<button type="default">搜索</button>
		</view>
		<!-- 轮播图 -->
		<view class="lunbo">
			<swiper :indicator-dots="true" :autoplay="true" :interval="3000" :duration="1000" circular="true">
				<swiper-item>
					<image src="https://aecpm.alicdn.com/simba/img/TB1X6uHLVXXXXcCXVXXSutbFXXX.jpg" mode=""></image>
				</swiper-item>
				<swiper-item>
					<image src="https://aecpm.alicdn.com/simba/img/TB13xKuLVXXXXcHapXXSutbFXXX.jpg" mode=""></image>
				</swiper-item>
				<swiper-item>
					<image src="//img.alicdn.com/tps/i4/TB1GrDgf8Bh1e4jSZFhSuwC9VXa.jpg_240x240q90.jpg" mode=""></image>
				</swiper-item>
			</swiper>
		</view>
		<view class="" style="margin-top:20px;">
			<view style="font-size:18px;font-weight:500;">您目前的位置是</view>
			<map :latitude="latitude" :longitude="longitude"></map>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				href: 'https://uniapp.dcloud.io/component/README?id=uniui'
			}
		},
		methods: {

		}
	}
</script>

<style>
	.container {
		font-size: 14px;
		line-height: 24px;
	}
	.search{
		margin-top:10px;
		padding-left:15px;
	}
	.search button{
		float:right;
		width:20%;
		height:30px;
		line-height:30px;
	}
	.lunbo image{
		width:100%;
	}
	map{
		width:100%;
		height:100px;
	}
</style>
