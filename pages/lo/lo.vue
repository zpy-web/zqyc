<template>
	<view>
		<!-- logo -->
		<view class="logo">
			<image src="../../static/login/icon_logo.png" mode=""></image>
		</view>
		<!-- 注册 -->
		<view class="login">
			<view class="login-s">
				<image src="../../static/login/icon_iphone_dl.png" mode=""></image>
				<input type="text" value="请输入手机号" />
			</view>
			<view class="login-s login-t">
				<image src="../../static/login/icon_password_dl.png" mode=""></image>
				<input type="text" value="请输入密码" />
			</view>
			<view class="duanxin login-s">
				<text>短信登录</text>
				<text>找回密码</text>
			</view>
		</view>
		<!-- 按钮 -->
		<view class="register">
			<view class="yes">
				<view class="yes-s">
					<image src="../../static/login/icon_dh-dl.png"></image>
				</view>
				<text>同意用户协议</text>
			</view>
			<view class="register-c">
				<view class="register-s">
					<text>登录</text>
				</view>
				<view class="register-s">
					<text>注册</text>
				</view>
			</view>
		</view>
		<!-- 第三方登录 -->
		<view class="footer">
			<view class="footer-b">
				第三方登录
			</view>
			<view class="footer-r">
				<view class="footer-rs">
					<image src="../../static/login/icon_wx_dl.png" mode=""></image>
				</view>
				<view class="footer-rs">
					<image src="../../static/login/icon_qq_dl.png" mode=""></image>
				</view>
				
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
page{background: #000000;}
.logo{
	
	display: flex;
	justify-content: center;
	align-items: center;
	height: 380rpx;
	width: 100%;
	image{
		width: 166rpx;
		height: 166rpx;
	}
}
.login{
	height: 260rpx;
	width: 100%;
	align-items: center;
	display: flex;
	flex-direction: column;
	font-size: 28rpx;
	color: #919191;
	.login-s{
		width: 630rpx;
		flex-direction: row;
		display: flex;
		border-bottom: 1rpx solid #919191;
		height: 66rpx;
		align-items: center;
		input{
			margin-left: 30rpx;
		}
	}
	.login-t{
		margin-top: 48rpx;
		
	}
	image{
		width: 40rpx;
		height: 48rpx;
	}
	.duanxin{
		margin-top: 10rpx;
		display: flex;
		justify-content: space-between;
		flex-direction: row;
		border: 0;
	}
}
.register{
	width: 630rpx;
	justify-content: center;
	margin: 0 auto;
	height: 390rpx;
	display: flex;
	flex-direction: column;
	font-size: 28rpx;
	.yes{
		display: flex;
		flex-direction: row;
		margin-left: 10rpx;
		text{
			margin-left: 10rpx;margin-top: -5rpx;
			color: #fff;
			font-size: 26rpx;
		}
		.yes-s{
			border-radius: 50%;
			background-color: red;
			width: 32rpx;
			height: 32rpx;
			text-align: center;
			line-height: 32rpx;
			image{
				width: 28rpx;
				height: 28rpx;
			}
		}
	}
	.register-c{
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		font-size: 32rpx;
		
	}
	.register-s{
		width: 623rpx;
		height: 80rpx;
		background: url(../../static/login/login_btn.png);
		background-size: 100% 100%;
		text-align: center;
		line-height: 80rpx;
		color: #fff;
		margin-top: 26rpx;
	}
}
.footer{
	width: 100%;
	height: 200rpx;
	display: flex;
	flex-direction: column;
	.footer-b{
		color: #4c4c4c;
		margin: 0 auto;
		width: 90%;
		height: 34rpx;
		background: url(../../static/login/img_hr_dl.png);
		background-repeat: no-repeat;
		background-size:100% 1rpx;
		background-position: center;
		text-align: center;
		line-height: 34rpx;
		font-size: 28rpx;
	}
	.footer-r{
		display: flex;
		flex-direction: row;
		width: 100%;
		height: 166rpx;
		.footer-rs{
			width: 50%;
			display: flex;
			justify-content: center;
			align-items: center;
		}
		image{
			width: 86rpx;
			height: 86rpx;
		}
	}
}
</style>
