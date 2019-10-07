<template>
	<!-- 18-消息内容 -->
	<view>
		<view class="massage">
			<text>2019-10-05&nbsp;22:39:45</text>
			<text class="fonts">
				系统消息系统消息系统消息系统消息系统消息系统消息
				系统消息系统消息系统消息系统消息系统消息系统消息
				系统消息系统消息系统消息系统消息系统消息系统消息
				系统消息系统消息系统消息系统消息系统消息系统消息
				系统消息系统消息系统消息。
			</text>
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
page{background-color: #f5f4f9;}
.massage{
	height: 290rpx;
	margin-top:20rpx;
	background-color: #fff;
	display: flex;
	width: 100%;
	justify-content: center;
	flex-direction: column;
	flex-wrap: wrap;
	text{
		font-size: 28rpx;
		color: #b5b4b9;
		margin-left: 30rpx;
	}
	.font{
		margin-top: 24rpx;
	}
}
</style>
