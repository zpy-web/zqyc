<template>
	<view class="content">
		<!-- logo -->
		<view class="logo">
			<image src="../../static/login/icon_logo.png" mode=""></image>
		</view>
		<!-- 注册 -->
		<view class="login">
			<view class="login-s">
				<image src="../../static/login/icon_iphone_dl.png" mode=""></image>
				<input type="number" focus="true" placeholder="请输入手机号" />
			</view>
			<view class="login-s login-t">
				<image src="../../static/login2/icon_yzm_dl2.png" mode=""></image>
				<input type="text" password="password" placeholder="请输入验证码" />
				<view class="code">获取验证码</view>
			</view>
		</view>
		<view class="login-b">
			登录
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
	page {
		background: #000000;
	}
		.logo {
			display: flex;
			justify-content: center;
			align-items: center;
			height: 380rpx;
			width: 100%;

			image {
				width: 166rpx;
				height: 166rpx;
			}
		}
		.login {
			height: 200rpx;
			width: 100%;
			align-items: center;
			display: flex;
			flex-direction: column;
			font-size: 28rpx;
			color: #919191;
			
			.login-s {
				width: 630rpx;
				flex-direction: row;
				display: flex;
				border-bottom: 1rpx solid #919191;
				height: 66rpx;
				align-items: center;

				input {
					margin-left: 30rpx;
				}
			}

			.login-t {
				margin-top: 54rpx;
				image{height: 30rpx;}
			}

			image {
				width: 40rpx;
				height: 48rpx;
			}
			.code{
				width: 172rpx;
				height: 60rpx;
				background-color: #ea303d;
				border-radius: 30rpx;
				font-size: 26rpx;
				text-align: center;
				line-height: 60rpx;
				color: #fedbe1;
				margin-left: 30rpx;
				margin-top: -20rpx;
			}

		}
	.login-b{
		margin: 0 auto;
		margin-top: 150rpx;
		width: 630rpx;
		height: 86rpx;
		background: url(../../static/login/login_btn.png) no-repeat;
		background-size: 100%;
		color: #fff;
		text-align: center;
		line-height: 86rpx;
	}
</style>
