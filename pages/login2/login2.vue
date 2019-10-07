<template>
	<!-- 2 -->
	<view>
		<!-- 登陆 logo -->
		<view class="header">
			<image src="../../static/login/icon_logo.png" mode=""></image>
		</view>
		<!-- ipone+password+短信 -->
		<view class="banner">
			<view class="banner-s">
				<view class="banner-s1">
					<image src="../../static/login/icon_iphone_dl.png" mode=""></image>
					<input type="text" value="请输入手机号" />
				</view>
				<view class="banner-s2">
					<image src="../../static/login2/icon_yzm_dl2.png" mode=""></image>
					<input type="text" value="请输入密码" />
					<!-- 获取验证吗 -->
					<view class="code">
						获取验证码
					</view>
				</view>
			</view>
		</view>
		<!-- 登录 -->
		<view class="login">
			<text>登录</text>
		</view>
	</view>
</template>
	</view>
<script>
	export default {
		data() {
			return {

			}
		},
		methods: {

		}
	}
</script>

<style>
page{background-color: #000;}
	/* 登陆 logo */
	/* ipone+password+短信 */
	.header{
		height: 208rpx;
		width: 100%;
		display: flex;
		justify-content: center;
		
	}
	.header image{
		width: 166rpx;
		height: 166rpx;
		margin-top: 42rpx;
	}
	.banner{
		height: 364rpx;
		width: 100%;
		padding-top: 110rpx;
		box-sizing: border-box;
	}
	.banner .banner-s{
		height: 254rpx;
		width: 634rpx;
		margin-left: 54rpx;
		display: flex;
		flex-direction: column;
	}
	/* 第一个 */
	.banner .banner-s .banner-s1{
		width: 100%;
		height: 60rpx;
		display: flex;
		border-bottom: 2rpx solid #bfbfbf;
		padding-left: 2rpx;
		box-sizing: border-box;
	}
	.banner .banner-s .banner-s1 image{
		width: 34rpx;
		height: 48rpx;
		margin-left: 2rpx;
	}
	.banner .banner-s .banner-s1 input{
		color: #9d9d9d;
		font-size: 28rpx;
		margin-left: 32rpx;
		
	}
	/* 第二个 */
	.banner .banner-s .banner-s2{
		width: 100%;
		height: 142rpx;
		border-bottom: 2rpx solid #bfbfbf;
		padding-left: 2rpx;
		box-sizing: border-box;
		display: flex;
	}
	.banner .banner-s .banner-s2 image{
		width: 38rpx;
		height: 26rpx;
		margin-left: 2rpx;
		margin-top: 100rpx;
	}
	.banner .banner-s .banner-s2 input{
		color: #9d9d9d;
		font-size: 28rpx;
		margin-left: 32rpx;
		margin-top: 88rpx;
	}
	.banner .banner-s .banner-s2 .code{
		margin-top: 60rpx;
		width: 172rpx;
		height: 60rpx;
		background-color: #ea303d;
		border-radius: 30rpx;
		font-size: 26rpx;
		text-align: center;
		line-height: 60rpx;
		color: #fedbe1;
		margin-left: 160rpx;
		}
		.login {
			display: flex;
			justify-content: center;
			height: 650rpx;
		}
		.login text{
			margin-top: 140rpx;
			width: 634rpx;
			height: 82rpx;
			background-image: url(../../static/login/login_btn.png);
			background-repeat: no-repeat;
			background-size: 100% 100%;
			font-size: 36rpx;
			text-align: center;
			line-height: 84rpx;
			color: #FFFFFF;
		}
</style>
	