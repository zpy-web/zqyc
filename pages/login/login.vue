<template>
	<!-- 1 -->
	<view>
		<view class="header">
			<image src="../../static/login/icon_logo.png" mode=""></image>
		</view>
		<view class="banner">
			<view class="banner-s">
				<view class="banner-s1">
					<image src="../../static/login/icon_iphone_dl.png" mode=""></image>
					<input type="text" value="请输入手机号" />
				</view>
				<view class="banner-s2">
					<image src="../../static/login/icon_password_dl.png" mode=""></image>
					<input type="text" value="请输入密码" />
				</view>
				<view class="banner-s3">
					<text>短信登陆</text>
					<text>找回密码</text>
				</view>
			</view>
		</view>
		<!-- login+register -->
		<view class="section">
				<view class="section-s">
					<view class="section-s1">
						<view class="yes">
							<image src="../../static/login/icon_dh-dl.png" mode="" style="width: 24rpx; height: 24rpx;"></image>
						</view>
						
						<text>同意用户协议</text>
					</view>
					<view class="section-s2">
						<view class="section-bg">登录</view>
						<view class="section-bg">注册</view>
					</view>
				</view>
				
		</view>
		<!-- 第三方登陆 -->
		<view class="others">
			<view class="lines"></view>
			<view class="fonts">
				第三方登录
			</view>
			<view class="lines"></view>
		</view>
		<!-- qq+wx -->
		<view class="footer">
			<image src="../../static/login/icon_wx_dl.png" mode=""></image>
			<image src="../../static/login/icon_qq_dl.png" mode=""></image>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		onLoad() {

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
		color: #bfbfbf;
		font-size: 28rpx;
		margin-left: 32rpx;
		
	}
	.banner .banner-s .banner-s2{
		width: 100%;
		height: 142rpx;
		border-bottom: 2rpx solid #bfbfbf;
		padding-left: 2rpx;
		box-sizing: border-box;
		display: flex;
	}
	.banner .banner-s .banner-s2 image{
		width: 40rpx;
		height: 48rpx;
		margin-left: 2rpx;
		margin-top: 80rpx;
	}
	.banner .banner-s .banner-s2 input{
		color: #bfbfbf;
		font-size: 28rpx;
		margin-left: 32rpx;
		margin-top: 88rpx;
		
	}
	.banner .banner-s .banner-s3{
		width: 100%;
		height: 52rpx;
		padding-top: 10rpx;
		box-sizing: border-box;
		font-size: 28rpx;
		color: #BFBFBF;
	}
	.banner .banner-s .banner-s3 text:first-child{float: left;}
	.banner .banner-s .banner-s3 text:last-child{float: right;}
	/* login+register */
	.section{width: 100%; height: 396rpx; display: flex; justify-content: center; align-items: center;}
	.section-s{width: 642rpx; height: 100%; }
	.section-s .section-s1{ height: 104rpx;padding-left: 20rpx;padding-top: 52rpx; box-sizing: border-box;display: flex;}
	.section-s .section-s1 .yes{
		width: 32rpx;
		height: 32rpx;
		background-image: url(../../static/login/icon_xy_dl.png);
		background-repeat: no-repeat;
		background-size: 100% 100%;
		text-align: center;
		line-height: 32rpx;
	}
	.section-s .section-s1 text{margin-left: 10rpx; font-size: 24rpx; color: #e8e8e8;}
	.section-s .section-s2{ height: 292rpx;}
	.section-s .section-s2 .section-bg{
		width: 640rpx;
		height: 84rpx;
		margin-top: 20rpx;
		background-image: url(../../static/login/login_btn.png);
		background-repeat: no-repeat;
		background-size: 100% 100%;
		font-size: 36rpx;
		text-align: center;
		line-height: 84rpx;
		color: #FFFFFF;
		}
	/* 第三方登陆  */
	.others{
		width: 90%;
		height:40rpx;
		margin: 30rpx auto;
		display: flex;
		justify-content: space-between;
		align-items: center;
	}
	.others .lines{
		width: 256rpx;
		height: 2rpx;
		background-color: #bfbfbf;
	}
	.others .fonts{
		color: #4c4c4c;
		font-size: 28rpx;
	}
	/* qq+wx */
	.footer{width: 100%;height: 102rpx;}
	.footer image{
		width: 86rpx;
		height: 86rpx;
		margin-left: 202rpx;
	}
</style>
