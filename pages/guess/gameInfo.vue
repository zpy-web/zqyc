<template>
	<!--  27-比赛记录-gameInfo-->
	<view>
		<!-- 2019-08-27比赛 -->
		<view class="gametop">
			<text>上一天</text>
			<text class="fonts">2019-08-27比赛</text>
			<text>下一天</text>
		</view>
		<!-- 内容 -->
		<view class="gamemain">
			<view class="main-s">
				<!-- 1 -->
				<view class="main1">
					<text>001</text>
					<text class="fontc">08-27&nbsp;23:35</text>
					<text>日职</text>
				</view>
				<!-- 2 -->
				<view class="main2">
					<text>广岛三箭</text>
					<text class="fontlr">VS</text>
					<text>广岛三箭</text>
				</view>
			</view>
		</view>
		<view class="gamemain">
			<view class="main-s">
				<view class="main1">
					<text>001</text>
					<text class="fontc">08-27&nbsp;23:35</text>
					<text>日职</text>
				</view>
				<view class="main2">
					<text>广岛三箭</text>
					<text class="fontlr">VS</text>
					<text>广岛三箭</text>
				</view>
			</view>
		</view>
		<view class="gamemain">
			<view class="main-s">
				<view class="main1">
					<text>001</text>
					<text class="fontc">08-27&nbsp;23:35</text>
					<text>日职</text>
				</view>
				<view class="main2">
					<text>广岛三箭</text>
					<text class="fontlr">VS</text>
					<text>广岛三箭</text>
				</view>
			</view>
		</view>
		<view class="gamemain">
			<view class="main-s">
				<view class="main1">
					<text>001</text>
					<text class="fontc">08-27&nbsp;23:35</text>
					<text>日职</text>
				</view>
				<view class="main2">
					<text>广岛三箭</text>
					<text class="fontlr">VS</text>
					<text>广岛三箭</text>
				</view>
			</view>
		</view>
		<view class="gamemain">
			<view class="main-s">
				<view class="main1">
					<text>001</text>
					<text class="fontc">08-27&nbsp;23:35</text>
					<text>日职</text>
				</view>
				<view class="main2">
					<text>广岛三箭</text>
					<text class="fontlr">VS</text>
					<text>广岛三箭</text>
				</view>
			</view>
		</view>
		<view class="gamemain">
			<view class="main-s">
				<view class="main1">
					<text>001</text>
					<text class="fontc">08-27&nbsp;23:35</text>
					<text>日职</text>
				</view>
				<view class="main2">
					<text>广岛三箭</text>
					<text class="fontlr">VS</text>
					<text>广岛三箭</text>
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
	page{
		background-color: #000;
		box-sizing: border-box;
	}
	// 头
.gametop{
	height: 100rpx;
	width: 100%;
	background-color: #201816;
	display: flex;
	justify-content: center;
	align-items: center;
	margin-bottom: 40rpx;
	text{
		color: #ffbc09;
		font-size: 28rpx;
	}
	.fonts{
		margin: 0 36rpx;
		color: #c4424a;
	}
}
// 内容
.gamemain{
	width: 100%;
	height: 150rpx;
	display: flex;
	justify-content: center;
	.main-s{
		width: 690rpx;
		height: 160rpx;
		border-bottom: 1rpx solid #303030;
		display: flex;
		flex-direction: column;
		// 1
		.main1{
			margin-top: 38rpx;
			display: flex;
			justify-content: space-around;
			text{
				color:#c4424a ;
				font-size: 26rpx;
			}
		}
		.fontc{
			color: #8b8b8b;
		}
		// 2
		.main2{
			margin-top: 38rpx;
			display: flex;
			justify-content: center;
			color: #fff;
			font-size: 28rpx;
			.fontlr{
				margin: 0 70rpx;
			}
		}
	}
}
</style>
