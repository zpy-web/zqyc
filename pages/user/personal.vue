<template>
	<!--6 个人主页 -->
	<view>
		<view class="header">
			<!-- <view class="pen"></view> -->
			<navigator :url="pdata" class="pen"></navigator>
			<image src="../../static/personal/img_tx_6grzx.png" mode=""></image>
			<text>Jocelyn</text>
		</view>
		<!-- 开通vip11090 -->
		<view class="vip">
			<view class="vip-s">
				<image src="../../static/personal/icon_ktvip_6grzx.png" mode=""></image>
				<text>开通VIP</text>
				<view>
					<navigator :url="openVip">开通</navigator>
				</view>
			</view>
		</view>
		<!-- 中间all -->
		<view class="section">
			<!-- 1 -->
			<!-- <view class="section-s"> -->
			<navigator :url="account" class="section-s">
				<image src="../../static/personal/icon_zhmx_6grzx.png" mode=""></image>
				<text>账户明细</text>
				<image class="last" src="../../static/personal/btn_enter.png" mode=""></image>
			</navigator>
			<!-- </view> -->
			<!-- 2 -->
			<view class="section-s" @click="openPopup">
				<image src="../../static/personal/icon_fxhy_6grzx.png" mode=""></image>
				<text>分享好友</text>
				<image class="last" src="../../static/personal/btn_enter.png" mode=""></image>
			</view>
			<!-- 3 -->
			<!-- <view class="section-s"> -->
			<navigator :url="cipone" class="section-s">
				<image src="../../static/personal/icon_hbsj_6grzx.png" mode="" style="height: 32rpx; width: 28rpx;"></image>
				<text>换绑手机</text>
				<image class="last" src="../../static/personal/btn_enter.png" mode=""></image>
			</navigator>
			<!-- </view> -->
			<!-- <view class="section-s"> -->
			<navigator :url="accountBind" class="section-s">
				<image src="../../static/personal/icon_zhbd_6grzx.png" mode=""></image>
				<text>账户绑定</text>
				<image class="last" src="../../static/personal/btn_enter.png" mode=""></image>
			</navigator>
			<!-- </view> -->
			<!-- <view class="section-s b-bottom"> -->
			<navigator :url="aboutUs" class="section-s b-bottom">
				<image src="../../static/personal/icon_gywm_6grzx.png" mode=""></image>
				<text>关于我们</text>
				<image class="last" src="../../static/personal/btn_enter.png" mode=""></image>
			</navigator>
			<!-- </view> -->
		</view>
		<view class="footer">
			<view class="">
				<text>退出登录</text>
			</view>
		</view>
		<uni-popup ref="popup" type="bottom" :custom="true">
					<view class="share">
						<text class="share-f">分享</text>
						<view class="share-s">
							<view class="share-fd">
								<image src="../../static/personal/icon_wx_6-2grzx.png" mode=""></image>
								<text>微信</text>
							</view>
							<view class="share-fd">
								<image src="../../static/personal/icon_pyq_6-2grzx.png" mode=""></image>
								<text>朋友圈</text>
							</view>
							<view class="share-fd">
								<image src="../../static/personal/icon_qq_6-2grzx.png" mode=""></image>
								<text>QQ</text>
							</view>
						</view>
					</view>
		</uni-popup>
	</view>
</template>

<script>
	import uniPopup from "@/components/uni-popup/uni-popup.vue"
	export default {
		components: {uniPopup},
		data() {
			return {
				// 修改个人资料
				pdata: '../user/pdata',
				// 开通vip
				openVip:'../user/openVip',
				// 账户明细
				account: '../user/account',
				// 换绑手机
				cipone:'../user/cipone',
				//账户绑定
				accountBind: '../user/accountBind',
				// 关于我们
				aboutUs: '../user/about-us'	
			}
		},
		methods:{
					openPopup(){
						this.$refs.popup.open()
					},
					closePopup(){
						this.$refs.popup.close()
					}
				}
	}
</script>

<style lang="scss">
	page {
		background-color: #f5f5f5;
	}

	// 顶部
	.header {
		width: 100%;
		height:336rpx;
		background-color: #000;
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
		position: relative;
		.pen {
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

		image {
			width: 196rpx;
			height: 196rpx;
			margin-left: -2rpx;
			margin-top: -2rpx;
		}

		text {
			font-size: 28rpx;
			color: #fff;
			margin-top: 10rpx;
		}

	}

	// vip开通
	.vip {
		background: #f5f5f5;
		width: 100%;
		height: 110rpx;
		display: flex;
		flex: 1;
		.vip-s {
			width: 100%;
			height: 90rpx;
			background-color: #fff;
			display: flex;
			align-items: center;
			image {
				width: 32rpx;
				height: 32rpx;
				margin-left: 30rpx;
			}

			text {
				font-size: 28rpx;
				margin-left: 20rpx;
			}

			view {
				background: url(../../static/personal/img_kt_6grzx.png);
				background-repeat: no-repeat;
				background-size: 100% 100%;
				margin-left: 410rpx;
				text-align: center;
				line-height: 50rpx;
				width: 120rpx;
				height: 50rpx;
				color: #fffeff;
				font-size: 28rpx;
			}
		}
	}

	// 中间部分
	.section {
		width: 100%;
		height: 452rpx;
		.section-s {
			width: 100%;
			height: 88rpx;
			display: flex;
			align-items: center;
			border-bottom: 1rpx solid #f5f5f5;
			background: #fff;
			image {
				width: 30rpx;
				height: 30rpx;
				margin-left: 30rpx;
			}

			text {
				font-size: 28rpx;
				margin-left: 22rpx;
			}

			.last {
				width: 14rpx;
				height: 24rpx;
				margin-left: 510rpx;
			}
		}

		.b-bottom {
			border-bottom: 0rpx;
		}
	}

	.footer {
		width: 100%;
		height: 308rpx;
		background-color: #f5f5f5;
		display: flex;
		justify-content: center;
		align-items: center;

		view {
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
	// 分享
	.share{
		height: 330rpx;
		width: 100%;
		background-color: #fff;
		border-radius: 20rpx 20rpx 0 0;
		.share-f{
			margin-left: 35rpx;
			font-size: 28rpx;
			height: 82rpx;
			width: 680rpx;
			display: flex;
			justify-content: center;
			align-items: center;
			border-bottom: 1rpx solid #f5f5f5;
		}
		.share-s{
			margin-left: 35rpx;
			width: 680rpx;
			height: 248rpx;
			display: flex;
			justify-content: space-around;
			align-items: center;
			.share-fd{
				display: flex;
				flex-direction: column;
				font-size: 28rpx;
				image{
					width: 80rpx;
					height: 80rpx;
				}
				text{
					margin-top: 14rpx;
					text-align: center;
				}
			}
		}
	}
</style>
