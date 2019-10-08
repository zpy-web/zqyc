<template>
	<!-- 21-账户绑定-Account binding -->
	<view>
		<view class="bind">
			<view class="bind-s">
				<image src="../../static/accountBind/icon_wx_21zhbd.png" mode=""></image>
				<text>绑定微信(获得1次解绑机会)</text>
			</view>
			<view class="bind-s bind-mt">
				<image src="../../static/accountBind/icon_wb_21zhbd.png" mode=""></image>
				<text>绑定微博(获得1次解绑机会)</text>
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
page{background-color: #f5f4f9;}
.bind{
	width: 100%;
	height: 240rpx;
	display: flex;
	justify-content: center;
	align-items: center;
	flex-direction: column;
	.bind-s{
		width:686rpx;
		height:90rpx;
		background-color: #fff;
		display: flex;
		justify-content: center;
		align-items: center;
		font-size: 28rpx;
		border-radius: 10rpx;
		image{
			width: 44rpx;
			height: 44rpx;
			margin-right: 20rpx;
		}
	}
	.bind-mt{margin-top: 20rpx;}
}
</style>
