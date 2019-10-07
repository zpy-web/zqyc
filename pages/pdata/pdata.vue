<template>
	<!-- 7 -->
	<view>
		<!-- 头像部分 -->
		<view class="head">
			<view class="head-s">
				<text>头像</text>
				<image class="img1" src="../../static/pdata/img_tx_7grzl.png" mode=""></image>
				<image class="img2" src="../../static/pdata/btn_enter_7grxx.png" mode=""></image>
			</view>
		</view>
		<!-- 昵称部分 -->
		<view class="section">
			<view class="section-s">
				<text>昵称</text>
				<text style="margin-left: 496rpx;">Jocelyn</text>
				<image src="../../static/pdata/btn_enter_7grxx.png" mode=""></image>
			</view>
			<!-- 修改密码 -->
			<view class="section-s">
				<text>修改密码</text>
				<image style="margin-left: 556rpx;" src="../../static/pdata/btn_enter_7grxx.png" mode=""></image>
			</view>
		</view>
	</view>
</template>

<script>

</script>

<style lang="scss">
	page{background-color: #f5f5f5;}
		// 头像
		.head {
			width: 100%;
			height: 200rpx;
			display: flex;
			align-items: center;

			.head-s {
				width: 100%;
				height: 160rpx;
				background-color: #fff;
				padding: 0 30rpx;
				box-sizing: border-box;
				display: flex;
				align-items: center;

				text {
					font-size: 28rpx;
					color: #9a9a9a;
				}

				.img1 {
					width: 122rpx;
					height: 122rpx;
					margin-left: 476rpx;
				}

				.img2 {
					width: 16rpx;
					height: 24rpx;
					margin-left: 20rpx;
				}
			}
		}
		// 昵称+pwd
		.section{
			box-sizing: border-box;
			height: 240rpx;
			background-color: #fff;
			padding: 0 30rpx;
			.section-s{
				height: 120rpx;
				width: 100%;
				display: flex;
				align-items: center;
				border-bottom: 2rpx solid #f5f5f5;
				text{
					font-size: 28rpx;
					color: #9a9a9a;
				}
				image {
					width: 16rpx;
					height: 24rpx;
					margin-left: 20rpx;
				}
			}
		
		}
</style>
