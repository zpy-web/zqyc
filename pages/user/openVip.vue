<template>
	<!-- 15 -->
	<view>
		<!-- 昵称 -->
		<view class="open">
			<image src="../../static/openVip/icon_nc_15ktvip.png" mode=""></image>
			<text>昵称:Jocelyn</text>
			<text class="open-s">免费次数&nbsp;:</text>
			<text class="open-s open-s2">1次</text>
		</view>
		<!-- 中间购买vip -->
		<view class="section">
			<view class="section-s">
				<view class="section-s1">
					<text>单次解锁</text>
					<text class="fcolor">10.00元</text>
				</view>
				<view class="section-s1 section-bg">
					<text>一个月</text>
					<text  class="fcolor">99.00元</text>
				</view>
				<view class="section-s1">
					<text>3个月</text>
					<text  class="fcolor">279.00元</text>
				</view>
				<view class="section-s1">
					<text>6个月</text>
					<text  class="fcolor">519.00元</text>
				</view>
			</view>
		</view>
		<!-- 购买 -->
		<view class="footer">
			<button @click="openPopup">购买</button>
		</view>
		<!-- 支付 -->
		<uni-popup ref="popup" type="bottom" :custom="true">
			<view class="payStyle">
				<view class="pay">
					
					<view class="fenx">
						<image src="../../static/openVip/icon_zffs_16zftc.png" mode=""></image>
						<text>请选择支付方式:</text>
					</view>
					<view class="pay-s">
						<view class="pay-s1">
							<image class="img-ml" src="../../static/openVip/icon_wxzf_16zftc.png" mode="">
								<text>微信支付</text>
							</image>
						</view>
						<view class="pay-s1">
						<image  src="../../static/openVip/icon_zfb_16zftc.png" mode=""><text>支付宝</text></image>
						</view>
					</view>
				</view>
				<button @click="closePopup">取消</button>
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
				
			};
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
	// 昵称
.open{
	height: 120rpx;
	width: 100%;
	background-color: #efeef3;
	display: flex;
	align-items: center;
	image{
		width: 42rpx;
		height: 42rpx;
		margin-left: 30rpx;
	}
	text{
		font-size: 28rpx;
		margin-left: 16rpx;
		color: #f57872;
	}
	.open-s{
		margin-left: 248rpx;
		color: #a2a2a4;
	}
	.open-s2{
		margin-left: 16rpx;
	}
}
// 中间消费
.section{
	height: 546rpx;
	width: 100%;
	display: flex;
	align-items: center;
	justify-content: center;
	.section-s{
		width: 688rpx;
		height: 428rpx;
		display: flex;
		justify-content:space-between;
		flex-wrap: wrap;
		.section-s1{
			width: 332rpx;
			height: 194rpx;
			background:url(../../static/openVip/img_bg_15ktvip.png);
			background-size: 100% 100%;
			background-repeat: no-repeat;
			display: flex;
			align-items: center;
			justify-content: center;
			flex-direction: column;
			text{
				margin-top: 20rpx;
				font-size: 30rpx;
			}
			.fcolor{
				color: #c34046;
			}
		}
		.section-bg{
			background:url(../../static/openVip/img_k_pre_15ktvip.png);
			background-size: 100% 100%;
			background-repeat: no-repeat;
		}
	}
}
// 购买
.footer{
	height: 212rpx;
	display: flex;
	justify-content: center;
	width: 100%;
	button{
		margin-top: 136rpx;
		height: 94rpx;
		width: 630rpx;
		background-color: #ea303d;
		border-radius: 47rpx;
		text-align: center;
		line-height: 94rpx;
		font-size: 36rpx;
		color: #fff;
	}
}
// 支付
.payStyle{
	width: 100%;
	height: 464rpx;
	display: flex;
	align-items: center;
	justify-content: center;
	flex-direction: column;
	font-size: 28rpx;
	.pay{
		background: #fff;
		width: 690rpx;
		height: 310rpx;
		border-radius: 20rpx;
		
		.fenx{
			width: 100%;
			height: 92rpx;
			display: flex;
			align-items: center;
			
			image{
				height: 32rpx;
				width: 6rpx;
				margin-left: 20rpx;
			}
			text{
				margin-left: 10rpx;
			}
		}
		.pay-s{
			border-top: 1rpx solid #f5f5f5;
			width: 100%;
			height: 218rpx;
			display: flex;
			align-items: center;
			justify-content: space-around;
			.pay-s1{
				display: flex;
				flex-direction: column;
				text{
					margin-top: 20rpx;
					font-size: 30rpx;
				}
				image{
					height: 74rpx;
					width: 74rpx;
					margin-left: 10rpx;
				}
				.img-ml{
					height: 70rpx;
					width: 86rpx;
					
				}
			}
		}
	}
	button{
		background: #fff;
		width: 690rpx;
		height: 110rpx;
		border-radius: 20rpx;
		margin-top: 20rpx;
		margin-bottom: 20rpx;
		text-align: center;
		line-height: 110rpx;
		color: #979797;
		font-size: 32rpx;
	}
}
</style>
