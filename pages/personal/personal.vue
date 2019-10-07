<template>
	<!--6  -->
	<view>
		<view class="header">
			<view class="pen"></view>
			<image src="../../static/personal/img_tx_6grzx.png" mode=""></image>
			<text>Jocelyn</text>
		</view>
		<!-- 开通vip11090 -->
		<view class="vip">
			<view class="vip-s">
				<image src="../../static/personal/icon_ktvip_6grzx.png" mode=""></image>
				<text>开通VIP</text>
				<view>开通</view>
			</view>
		</view>
		<!-- 中间all -->
		<view class="section">
			<!-- 1 -->
			<view class="section-s">
				<image src="../../static/personal/icon_zhmx_6grzx.png" mode=""></image>
				<text>账户明细</text>
				<image  class="last" src="../../static/personal/btn_enter.png" mode=""></image>
			</view>
			<!-- 2 -->
			<view class="section-s">
				<image src="../../static/personal/icon_fxhy_6grzx.png" mode=""></image>
				<text>分享好友</text>
				<image  class="last" src="../../static/personal/btn_enter.png" mode=""></image>
			</view>
			<!-- 3 -->
			<view class="section-s">
				<image src="../../static/personal/icon_hbsj_6grzx.png" mode="" style="height: 32rpx; width: 28rpx;"></image>
				<text>换绑手机</text>
				<image  class="last" src="../../static/personal/btn_enter.png" mode=""></image>
			</view>
			<view class="section-s">
				<image src="../../static/personal/icon_zhbd_6grzx.png" mode=""></image>
				<text>账户绑定</text>
				<image  class="last" src="../../static/personal/btn_enter.png" mode=""></image>
			</view>
			<view class="section-s b-bottom">
				<image src="../../static/personal/icon_gywm_6grzx.png" mode=""></image>
				<text>关于我们</text>
				<image  class="last" src="../../static/personal/btn_enter.png" mode=""></image>
			</view>
		</view>
		<view class="footer">
			<view class="">
				<text>退出登录</text>
			</view>
		</view>
	</view>
</template>

<script>
	
</script>

<style lang="scss">
	// 顶部
	.header{
		width: 100%;
		height: 336rpx;
		background-color: #000;
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
		position: relative;
		.pen{
			position: absolute;
			top: 50rpx;
			left: 464rpx;
				width: 42rpx;
				height: 42rpx;
				background: #e7313e;
				border-radius: 50%;
				background-image: url(../../static/personal/icon_qb_6grzx.png);
				background-size: 24rpx 24rpx;
				background-position: center;
				background-repeat: no-repeat;
		}
			image{
				width: 196rpx;
				height: 196rpx;
				margin-left: -2rpx;
				margin-top: -2rpx;
			}
			text{
				font-size: 28rpx;
				color: #fff;
				margin-top: 10rpx;
			}
			
		}
	// vip开通
	.vip{
		background: #f5f5f5;
		width: 100%;
		height: 110rpx;
		.vip-s{
			width: 100%;
			height: 90rpx;
			background-color: #fff;
			display: flex;
			align-items: center;
			image{
				width: 32rpx;
				height: 32rpx;
				margin-left: 30rpx;
			}
			text{
				font-size: 28rpx;
				margin-left: 20rpx;
			}
			view{
				background: url(../../static/personal/img_kt_6grzx.png);
				background-repeat: no-repeat;
				background-size: 100% 100%;
				margin-left: 410rpx;
				text-align: center;
				line-height: 50rpx;
				width:120rpx;
				height: 50rpx;
				color: #fffeff;
				font-size: 28rpx;
			}
		}
	}
	// 中间部分
	.section{
		width: 100%;
		height: 452rpx;
		.section-s{
			width: 100%;
			height: 88rpx;
			display: flex;
			align-items: center;
			border-bottom: 1rpx solid #f5f5f5;
			image{
				width: 30rpx;
				height: 30rpx;
				margin-left: 30rpx;
			}
			text{
				font-size: 28rpx;
				margin-left: 22rpx;
			}
			.last{
				width: 14rpx;
				height: 24rpx;
				margin-left: 510rpx;
			}
		}
		.b-bottom{
			border-bottom: 0rpx;
		}
	}
	.footer{
		width: 100%;
		height: 308rpx;
		background-color: #f5f5f5;
		display: flex;
		justify-content: center;
		align-items: center;
		view{
			background-image: url(../../static/personal/login_btn.png);
			width: 634rpx;
			height: 84rpx;
			background-size: 100% 100%;
			text-align: center;
			line-height: 84rpx;
			color: #fff2f7;
			font-size: 34rpx;
		}
	}
</style>
