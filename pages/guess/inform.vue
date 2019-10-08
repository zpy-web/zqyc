<template>
	<!-- 17 -->
	<view>
		<!-- top部分 -->
		<view class="inform">
			<text class="active">短消息</text>
			<text>系统通知</text>
		</view>
		<!-- 信息message -->
		<view class="message">
			<text>2019-10-05&nbsp;22:39:45</text>
			<text class="fonts">消息内容消息内容消息内容消息内容消息内容消息内容...</text>
		</view>
		<view class="message">
			<text>2019-10-05&nbsp;22:39:45</text>
			<text class="fonts">消息内容消息内容消息内容消息内容消息内容消息内容...</text>
		</view>
		<view class="message">
			<text>2019-10-05&nbsp;22:39:45</text>
			<text class="fonts">消息内容消息内容消息内容消息内容消息内容消息...</text>
		</view>
		<view class="message">
			<text>2019-10-05&nbsp;22:39:45</text>
			<text class="fonts">消息内容消息内容消息内容消息内容消息内容消息...</text>
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
	// 1
.inform{
	height: 100rpx;
	width: 100%;
	background-color: #efeef3;
	display: flex;
	align-items: center;
	justify-content: space-around;
	text{
		
		line-height: 100rpx;
		text-align: center;
		width: 50%;
		font-size: 30rpx;
		color: #b5b4b9;
	}
	// 点击是那条线
	.active{
		box-sizing: border-box;
		border-bottom: 4rpx solid #eb303b;
		color: #eb303b;
	}	
}
// 2
.message{
	height: 150rpx;
	width: 92%;
	display: flex;
	margin-left: 30rpx;
	justify-content: center;
	flex-wrap: wrap;
	flex-direction: column;
	border-bottom: 1rpx solid #f5f5f5;
	text{
		width: 100%;
		display: flex;
		font-size: 26rpx;
		color: #b5b4b9;
	}
	.fonts{
		margin-top: 20rpx;
	}
}
</style>
