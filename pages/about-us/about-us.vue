<template>
	<!-- 11 -->
	<view>
		<!-- logo -->
		<view class="about-us">
			<view class="logo">
				<image src="../../static/about-us/img_logo_11gywm.png" mode=""></image>
				<text>产品版本号：V2.0.1</text>
			</view>
		</view>
		<!-- 客服QQ:12345678 -->
		<view class="about-all">
			<view class="about-qq">
				<text>客服QQ:</text>
				<text style="margin-left: 18rpx;">12345678</text>
			</view>
		</view>
		<view class="about-all">
			<view class="about-qq">
				<text>商务合作:</text>
				<text style="margin-left: 18rpx;">12345678@qq.com</text>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			};
		}
	}
</script>

<style lang="scss">
.about-us{
	width: 100%;
	height: 300rpx;
	background-color: black;
	display: flex;
	align-items: center;
	justify-content: center;
	.logo{
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		image{
			width:166rpx;
			height: 166rpx;
		}
		text{
			margin-top: 10rpx;
			font-size: 30rpx;
			color: #fff;
		}
	}
}
.about-all{
	padding-left: 30rpx;
	box-sizing: border-box;
	height: 100rpx;
	width: 100%;
	display: flex;
	align-items: center;
	.about-qq{
		font-size: 28rpx;
		display: flex;
		align-items: center;
		height: 100rpx;
		width: 96%;
		border-bottom: 1rpx solid #f5f5f5;
	}
}
</style>
