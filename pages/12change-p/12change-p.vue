<template>
	<!-- 12 -->
	<view class="content">
		<!-- 手机 -->
		<view class="ipone">
			<view class="ipone-s">
				<image src="../../static/binding/icon_iphone_5bdsjh.png" mode=""></image>
				<input type="text" value="请输入手机号" />
			</view>
		</view>
		<!-- 手机2 -->
		<view class="ipone ipont-m">
			<view class="ipone-s">
				<image src="../../static/binding/icon_iphone_5bdsjh.png" mode=""></image>
				<input type="text" value="请输入新的手机号" />
			</view>
		</view>
		<!-- 验证码 -->
		<view class="code">
			<image src="../../static/binding/icon_yzm_5bdsjh.png" mode=""></image>
			<input type="text" value="请输入验证码" />
			<view>获取验证码</view>
		</view>
		<!-- 确定按钮 -->
		<view class="footer">
			<view>确定</view>
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
		page{background: #f5f5f5;}
		//手机
		.ipont-m{
			margin-top: -20rpx;
		}
		.ipone{
			height: 140rpx;
			width: 100%;
			display: flex;
			align-items: center;
			.ipone-s{
				width: 100%;
				height: 100rpx;
				background-color: #fff;
				display: flex;
				align-items: center;
				image{
					width:34rpx;
					height:44rpx;
					margin-left: 54rpx;
				}
				input{
					font-size: 28rpx;
					color: #979797;
					margin-left: 30rpx;
				}
			}
		}
		// 验证码
		.code{
			height: 100rpx;
			background-color: #fff;
			width: 100%;
			display: flex;
			align-items: center;
			image{
				width:36rpx;
				height:32rpx;
				margin-left: 54rpx;
			}
			input{
				font-size: 28rpx;
				color: #979797;
				margin-left: 30rpx;
			}
			view{
				width: 172rpx;
				height: 60rpx;
				background-color: #ea303d;
				border-radius: 30rpx;
				font-size: 26rpx;
				text-align: center;
				line-height: 60rpx;
				color: #fedbe1;
				margin-left: 120rpx;
			}
		}
		// 确定
		.footer{
			height: 968rpx;
			width: 100rpx;
			view{
				font-size: 30rpx;
				width:632rpx;
				height: 80rpx;
				background-image: url(../../static/binding/login_btn.png);
				background-repeat: no-repeat;
				background-size: 100% 100%;
				text-align: center;
				line-height: 80rpx;
				color: #fefdfb;
				margin-left: 58rpx;
				margin-top: 190rpx;
			}
		}
</style>
