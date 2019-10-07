<template>
	<!-- 9 -->
	<view>
		<view class="mtn">
			<text>请输入昵称</text>
		</view>
		<view class="mtn-x">
			<image src="../../static/9mtn/icon_gb_9xgnc.png" mode=""></image>
			<input type="text" value="Jocelyn">
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
page{
	background-color: #f5f5f5;
}
// 请输入昵称
.mtn{
	width: 100%;
	height: 66rpx;
	display: flex;
	align-items: center;
	
	text{
		font-size: 24rpx;
		color: #c3c3c3;
		margin-left: 30rpx;
	}
}
.mtn-x{
		width: 100%;
		height: 120rpx;
		display: flex;
		align-items: center;
		background-color: #fff;
		image{
			height: 46rpx;
			width: 5rpx;
			margin-left: 30rpx;
		}
		input{
			font-size: 28rpx;
			color: #000;
		}
	}

</style>
