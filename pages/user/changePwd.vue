<template>
	<!-- 10 -->
	<view>
		<!--请输入原密码  -->
		<view class="changepwd">
			<view class="changepwd-s">
				<image src="../../static/changePwd/icon_password_10xgmm.png"></image>
				<input type="text"  value="请输入原密码">
			</view>
		</view>
		<!-- 请输入新密码 -->
		<view class="changepwd-s2">
			<image src="../../static/changePwd/icon_password_10xgmm.png"></image>
			<input type="text"  value="请输入新密码">
		</view>
		<!-- queding -->
		<view class="changepwd-yes">确定</view>
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
.changepwd{
	width: 100%;
	height: 140rpx;
	display: flex;
	align-items: center;
	.changepwd-s{
		width: 100%;
		height: 100rpx;
		background-color: #fff;
		display: flex;
		align-items: center;
		image{
			margin-left: 28rpx;
			height:36rpx;
			width: 32rpx;
		}
		input{
			color: #9e9e9e;
			font-size: 28rpx;
			margin-left: 34rpx;
		}
	}
}
.changepwd-s2{
		width: 100%;
		height: 100rpx;
		background-color: #fff;
		display: flex;
		align-items: center;
		image{
			margin-left: 28rpx;
			height:36rpx;
			width: 32rpx;
		}
		input{
			color: #9e9e9e;
			font-size: 28rpx;
			margin-left: 34rpx;
		}
	}
	.changepwd-yes{
		width: 100%;
		height: 200rpx;
		background-color: #007AFF;
	}
.changepwd-yes{
	width: 634rpx;
	height: 82rpx;
	background-color: #ea303d;
	border-radius: 41rpx;
	margin-top: 188rpx;
	margin-left: 60rpx;
	text-align: center;
	line-height: 82rpx;
	color: #fff;
}
</style>
