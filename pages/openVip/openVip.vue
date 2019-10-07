<template>
	<!-- 15 -->
	<view>
		<!-- 昵称 -->
		<view class="open">
			<image src="../../static/openVip/icon_nc_15ktvip.png" mode=""></image>
			<text>昵称:Jocelyn</text>
			<text class="open-s">免费次数&nbsp;:</text>
			<text class="open-s open-s2">1次</text>
		</view>
		<!-- 中间购买vip -->
		<view class="section">
			<view class="section-s">
				<view class="section-s1">
					<text>单次解锁</text>
					<text class="fcolor">10.00元</text>
				</view>
				<view class="section-s1 section-bg">
					<text>一个月</text>
					<text  class="fcolor">99.00元</text>
				</view>
				<view class="section-s1">
					<text>3个月</text>
					<text  class="fcolor">279.00元</text>
				</view>
				<view class="section-s1">
					<text>6个月</text>
					<text  class="fcolor">519.00元</text>
				</view>
			</view>
		</view>
		<!-- 购买 -->
		<view class="footer">
			<view>购买</view>
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
	// 昵称
.open{
	height: 120rpx;
	width: 100%;
	background-color: #efeef3;
	display: flex;
	align-items: center;
	image{
		width: 42rpx;
		height: 42rpx;
		margin-left: 30rpx;
	}
	text{
		font-size: 28rpx;
		margin-left: 16rpx;
		color: #f57872;
	}
	.open-s{
		margin-left: 248rpx;
		color: #a2a2a4;
	}
	.open-s2{
		margin-left: 16rpx;
	}
}
// 中间消费
.section{
	height: 546rpx;
	width: 100%;
	display: flex;
	align-items: center;
	justify-content: center;
	.section-s{
		width: 688rpx;
		height: 428rpx;
		display: flex;
		justify-content:space-between;
		flex-wrap: wrap;
		.section-s1{
			width: 332rpx;
			height: 194rpx;
			background:url(../../static/openVip/img_bg_15ktvip.png);
			background-size: 100% 100%;
			background-repeat: no-repeat;
			display: flex;
			align-items: center;
			justify-content: center;
			flex-direction: column;
			text{
				margin-top: 20rpx;
				font-size: 30rpx;
			}
			.fcolor{
				color: #c34046;
			}
		}
		.section-bg{
			background:url(../../static/openVip/img_k_pre_15ktvip.png);
			background-size: 100% 100%;
			background-repeat: no-repeat;
		}
	}
}
// 购买
.footer{
	height: 212rpx;
	display: flex;
	justify-content: center;
	width: 100%;
	view{
		margin-top: 118rpx;
		height: 94rpx;
		width: 630rpx;
		background-color: #ea303d;
		border-radius: 47rpx;
		text-align: center;
		line-height: 94rpx;
		font-size: 36rpx;
		color: #fff;
	}
}
</style>
