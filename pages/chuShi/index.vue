<template>
	<view id="chuShi">
		<!-- 轮播图 -->
		<swiper class="swiper" indicator-dots autoplay interval="2000" duration="500">
			<swiper-item><image class="swiperImg" src="https://aecpm.alicdn.com/simba/img/TB183NQapLM8KJjSZFBSutJHVXa.jpg" mode=""></image></swiper-item>
			<swiper-item><image class="swiperImg" src="https://aecpm.alicdn.com/simba/img/TB1XotJXQfb_uJkSnhJSuvdDVXa.jpg" mode=""></image></swiper-item>
			<swiper-item><image class="swiperImg" src="https://aecpm.alicdn.com/simba/img/TB1JNHwKFXXXXafXVXXSutbFXXX.jpg" mode=""></image></swiper-item>
		</swiper>
		<!-- 导航栏 -->
		<view class="nav">
			<view class="one" v-for="(item, index) in 4" :key="index">
				<image class="img" src="//img.alicdn.com/tps/i4/TB1zkDeIFXXXXXrXVXX07tlTXXX-200-200.png_60x60.jpg_.webp"></image>
				<text>书院结构</text>
			</view>
		</view>
		<!-- 旅游风景 -->
		<view class="scenery" v-for="(item,index) in 3" :key = "index">
			<image src="//img.alicdn.com/tfs/TB11ddWHXY7gK0jSZKzXXaikpXa-520-280.jpg_q90_.webp" mode=""></image>
			<text>罗天岩</text>
			<view class=""></view>
		</view>
	</view>
</template>

<script>
export default {
	data() {
		return {};
	},
	onLoad() {},
	methods: {}
};
</script>

<style lang="less">
// 轮播图
#chuShi {
	width: 100%;
	background-color: #7bc88b;
	.swiper {
		.swiperImg {
			width: 100%;
			height: 300rpx;
		}
	}
}

// 导航栏
.nav {
	display: flex;
	box-sizing: border-box;
	justify-content: space-between;
	align-items: center;
	width: 100%;
	height: 220rpx;
	padding: 30rpx;
	.one {
		width: 23%;
		height: 100%;
		text-align: center;
		.img {
			width: 107rpx;
			height: 107rpx;
			display: block;
			margin: 0 auto;
			margin-bottom: 10rpx;
		}
		text {
			font-size: 13px;
			color: #fff;
		}
	}
}

// 旅游风景
.scenery {
	width: 100%;
	height: 440rpx;
	padding: 30rpx;
	box-sizing: border-box;
	image {
		width: 100%;
		height: 350rpx;
	}
	text {
		font-size: 13px;
		color: #fff;
	}
	view {
		width: 100%;
		border: 1px solid #fff;
		margin-top: 5rpx;
	}
}
</style>
