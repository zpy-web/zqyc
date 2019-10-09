<template>
	<!-- 13-竞猜首页 -->
	<view >
		 <view class="status_bar">
		      <!-- 状态 -->
		 </view>
		 <view class="navigationBar">
			 <navigator url="inform"><image  src="../../static/13guessIndex/icon_xxtz_13jcsy.png" mode=""></image></navigator>
			 <text>软件名称</text>
			 <navigator :url="personal"><image src="../../static/13guessIndex/icon_qcy_13jcsy.png" mode=""></image></navigator>
		 </view> 
		<view class="body">
			<!-- 对话1 -->
			<view class="guess-logo">
				<image src="../../static/13guessIndex/img1_13jcsy.png"></image>
				<view class="text-bg"><text>软件介绍：XXXXXXXXXX</text></view>
			</view>
			<!-- 客服 -->
			<view class="guess-text">
				<text>客服微信：123456789</text>
			</view>
			<!-- 对话2 -->
			<view class="guess-logo guess-mt">
				<image src="../../static/13guessIndex/img1_13jcsy.png"></image>
				<view class="text-bg voice">语音4"</view>
			</view>
			<!-- 对话3 -->
			<view class="guess-person">
				<view class="person-fonts">
					我发送的信息
				</view>
				<image src="../../static/13guessIndex/img2_13jcsy.png" mode=""></image>
			</view>
			<!-- 球 -->
			<view class="ball">
				<navigator url="liveEvent">
					<image src="../../static/13guessIndex/icon_zq_13jcsy.png" mode=""></image>
				</navigator>
			</view>
		</view>
		<view class="footer">
			<image src="../../static/13guessIndex/icon_yy_13jcsy.png" mode=""></image>
			<view class="input">
				<image src="../../static/13guessIndex/icon_sr_13jcsy.png" mode=""></image>
				<input type="text" value="请输入...您的需求" />
			</view>
			<image src="../../static/13guessIndex/icon_xx_13jcsy.png" mode=""></image>
			<image src="../../static/13guessIndex/icon_tj_13jcsy.png" mode=""></image>
		</view>
		
	</view>
</template>

<script>
	export default{
		data(){
			return{
				personal:'../user/personal'
			}
		}
	}
</script>

<style lang="scss">
	page {
		background-color: #f5f4f9;
	}
	 .status_bar {
	      height: var(--status-bar-height);
	      width: 100%;
		  background-color: #000000;
	  }
	.navigationBar{
		height: 88rpx;
		width: 100%;
		background-color: #000000;
		color: #fff;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 0 30rpx;
		box-sizing: border-box;
		font-size: 32rpx;
		image{
			height: 42rpx;
			width: 42rpx;
		}
	}
	.body {
		
		margin-top: 32rpx;
		margin-left: 30rpx;
		// 对话1
		.guess-logo {
			display: flex;
			flex-wrap: nowrap;

			image {
				width: 88rpx;
				height: 88rpx;
			}

			.text-bg {
				background: url(../../static/guess/img_qpbg1_13jcsy.png);
				width: 422rpx;
				text-align: center;
				line-height: 86rpx;
				height: 86rpx;
				font-size: 30rpx;

				text {
					margin-left: 34rpx;
				}
			}
			.voice {
				width: 190rpx;

			}
		}
		.guess-mt {
			margin-top: 50rpx;
		}

		// 客服
		.guess-text {
			width: 420rpx;
			height: 80rpx;
			background: url(../../static/guess/img_bg_kfwx_13jcsy.png);
			text-align: center;
			line-height: 80rpx;
			font-size: 30rpx;
			margin-left: 300rpx;
			margin-top: 16rpx;
			background-size: 100% 100%;
			background-repeat: no-repeat;
			color: #909090;
		}

		// 对象4person
		.guess-person {
			width: 362rpx;
			height: 88rpx;
			margin-left: 328rpx;
			margin-top: 46rpx;
			display: flex;
			flex-wrap: nowrap;
			view {
				background: url(../../static/13guessIndex/img_qpbg3_13jcsy.png);
				text-align: center;
				background-size: 100% 100%;
				line-height: 86rpx;
				width: 260rpx;
				height: 86rpx;
				margin-right: 10rpx;
				color: #fff;
				font-size: 28rpx;
			}

			image {
				width: 88rpx;
				height: 88rpx;
			}
		}

		.ball {
			margin-top: 454rpx;

			image {
				width: 130rpx;
				height: 106rpx;
			}
		}
	}

	.footer {
		margin-top: 44rpx;
		height: 100rpx;
		background-color: #fff;
		display: flex;
		align-items: center;
		justify-content: space-around;

		image {
			width: 40rpx;
			height: 38rpx;
		}

		view {
			display: flex;
			flex-wrap: nowrap;
			width: 478rpx;
			height: 66rpx;
			box-sizing: border-box;
			border: 1rpx solid #eee;
			align-items: center;
			font-size: 24rpx;
			color: #565656;
			image{
				width: 26rpx;
				height: 26rpx;
				margin-left: 14rpx;
				margin-right: 14rpx;
			}
		}
	}
</style>
