<template>
	<view>
		<view class="main">
			<view class="main-s">
				<text class="font1">19:30开赛|亚冠</text>
				<text>队伍A&nbsp;VS&nbsp;队伍B</text>
				<text class="font2">比分&nbsp;&nbsp;1&nbsp;:&nbsp;5</text>
			</view>
		</view>
		<view class="section">
			<view class="section-s">
				<text class="section-s1">19:30开赛|亚冠</text>
				<text class="section-s2">预计23:05开启</text>
				<text class="section-s3">队伍A&nbsp;VS&nbsp;队伍B</text>
			</view>
		</view>
		<view class="section">
			<view class="section-s">
				<text class="section-s1">19:30开赛|亚冠</text>
				<text class="section-s2">预计23:05开启</text>
				<text class="section-s3">队伍A&nbsp;VS&nbsp;队伍B</text>
			</view>
		</view>
		<view class="section">
			<view class="section-s">
				<text class="section-s1">19:30开赛|亚冠</text>
				<text class="section-s2">预计23:05开启</text>
				<text class="section-s3">队伍A&nbsp;VS&nbsp;队伍B</text>
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
page{background: #f5f4f9;}
.main{
	height: 180rpx;
	width: 100%;
	display: flex;
	align-items: center;
	.main-s{
		display: flex;
		width: 100%;
		height: 138rpx;
		background-color: #fff;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		font-size: 28rpx;
		.font1{
			margin-left: -520rpx;
			font-size: 26rpx;
			color: #9b9b9b;
		}
	}
}
.section{
	height: 180rpx;
	width: 100%;
	display: flex;
	align-items: center;
	margin-top: -20rpx;
	.section-s{
		background: #fff;
		width: 100%;
		height: 138rpx;
		font-size: 28rpx;
		.section-s1{
			font-size: 26rpx;
			color:  #9b9b9b;
			float: left; margin-left: 30rpx;margin-top: 20rpx;
		}
		.section-s2{
			font-size: 26rpx;
			margin-top: 20rpx;
			float: right; margin-right: 30rpx;
		}
		.section-s3{
			display: block;
			height: 100%;
			width: 100%;
			text-align: center; line-height: 138rpx;
		}
	}
}

</style>
