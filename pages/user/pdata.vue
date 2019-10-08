<template>
	<!-- 7 -->
	<view>
		<!-- 头像部分 -->
		<view class="head">
			<view class="head-s">
				<text>头像</text>
				<image @click="openPopup" class="img1" src="../../static/pdata/img_tx_7grzl.png" mode=""></image>
				<image class="img2" src="../../static/pdata/btn_enter_7grxx.png" mode=""></image>
			</view>
		</view>
		<!-- 昵称部分 -->
		<view class="section">
			<!-- <view class="section-s"> -->
			<navigator :url="mtn" class="section-s">
				<text>昵称</text>
				<text style="margin-left: 496rpx;">Jocelyn</text>
				<image src="../../static/pdata/btn_enter_7grxx.png" mode=""></image>
			</navigator>
			<!-- </view> -->
			<!-- 修改密码 -->
			<!-- <view class="section-s"> -->
			<navigator :url="changePwd" class="section-s">
				<text>修改密码</text>
				<image style="margin-left: 556rpx;" src="../../static/pdata/btn_enter_7grxx.png" mode=""></image>
		<!-- 	</view> -->
			</navigator>
		</view>
		<!-- 弹出 -->
				<uni-popup ref="popup" type="bottom" :custom="true">
					<view class="body">
						<view class="photo">
							<view class="photo-f photo-f1">
								<text>拍摄</text>
								<text class="small">照片或视频</text>
							</view>
							<view class="photo-f">
								<text>从手机相册选择</text>
							</view>
						</view>
						<button @click="closePopup">取消</button>
					</view>
				</uni-popup>
	</view>
	<!-- toux -->
	
</template>

<script>
	import uniPopup from "@/components/uni-popup/uni-popup.vue"
	export default {
		components: {
			uniPopup
		},
		data() {
			return {
				mtn:'../user/mtn',
				changePwd:'../user/changePwd'
			};
		},
		methods: {
			openPopup() {
				this.$refs.popup.open()
				console.log('dianji')
			},
			closePopup() {
				this.$refs.popup.close()
			}
		}
	}
</script>

<style lang="scss">
	page {
		background-color: #f5f5f5;
	}

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
	.section {
		box-sizing: border-box;
		height: 240rpx;
		background-color: #fff;
		padding: 0 30rpx;

		.section-s {
			height: 120rpx;
			width: 100%;
			display: flex;
			align-items: center;
			border-bottom: 2rpx solid #f5f5f5;

			text {
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
	.payStyle{
		width: 100%;
		height: 200rpx;
		background: #000000;
	}
// 弹出
.body{
	width: 100%;
	display: flex;
	align-items: center;
	justify-content: center;
	height: 410rpx;
	flex-direction: column;
	.photo{
		border-radius:20rpx;
		height: 240rpx;
		width: 690rpx;
		background-color: #fff;
		.photo-f{
			font-size: 30rpx;
			display: flex;
			justify-content: center;
			align-items: center;
			width: 100%;
			height: 120rpx;
		}
		.photo-f1{
			display: flex;
			flex-direction: column;
			border-bottom: 1rpx solid #eee;
			.small{
				font-size: 28rpx;
				color:#9e9e9e ;
			}
		}
	}
	button{
		background: #fff;
		width: 690rpx;
		height: 110rpx;
		border-radius: 20rpx;
		margin-top: 30rpx;
		margin-bottom: 30rpx;
		text-align: center;
		line-height: 110rpx;
		color: #979797;
		font-size: 32rpx;
	}
}

</style>
