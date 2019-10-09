<template>
	<view>
		<!-- 自定义导航 -->
		<view class="status_bar">
			<!-- 状态 -->
		</view>
		<view class="navigationBar">
					 <image @tap="back" class="back"  src="../../static/13guessIndex/icon_back_dl2.png" mode=""></image>
					 <text>软件名称</text>
					 <image @click="show('right')" src="../../static/13guessIndex/icon_sx_23sszb.png" mode=""></image>
		</view> 
		<!-- 直播 -->
		<uni-drawer :visible="showRigth" mode="right" @close="closeDrawer('right')">
			<view class="aside">
				<view class="option" v-for="(list,i) in lists":key="i">
					{{list}}
				</view>
				
			</view>
		</uni-drawer>
		<!-- 文字 -->
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
	import uniDrawer from '@/components/uni-drawer/uni-drawer.vue'
	export default {
		components: {	
			uniDrawer
		},
		data() {
			return {
				showRigth: false,
				lists:['美职足','俄超','瑞超','俄超','亚冠','荷乙','德乙','意甲','法乙','巴西']
			}
		},
		methods: {
			back(){
				uni.navigateTo({
					url:'guessIndex'
				})
			},
			show(e) {
					this.showRigth = true
			},
			hide() {
				this.showLeft = false
				this.showRigth = false
			},
			closeDrawer(e) {
				if (e === 'left') {
					this.showLeft = false
				} else {
					this.showRigth = false
				}
			}
		}
	}
</script>

<style lang="scss">
	page {
		background: #f5f4f9;
	}
	// 自定义导航
	.status_bar {
	      height: var(--status-bar-height);
	      width: 100%;
		  background-color: #000000;
	  }
	.navigationBar{
		height: 88rpx;
		width: 100%;
		background-color: #000000;
		color: #fff;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 0 30rpx;
		box-sizing: border-box;
		font-size: 32rpx;
		.back{
			height: 30rpx;
			width: 18rpx;
		}
		image{
			height: 34rpx;
			width: 36rpx;
		}
	}
	//侧边栏
	.aside{
		// height: 100%;
		padding: 10rpx 20rpx;
		box-sizing: border-box;
		display: flex;
		justify-content: space-between;
		flex-wrap: wrap;
		.option{
			margin-right: 10rpx;
			margin-top: 20rpx;
			width:220rpx;
			height:66rpx;
			border: 1rpx solid red;
			border-radius: 33rpx;
			text-align: center;
			line-height: 66rpx;
			color: #000;
			font-size: 28rpx;
		}
	}
	// 主体
	.main {
		height: 180rpx;
		width: 100%;
		display: flex;
		align-items: center;

		.main-s {
			display: flex;
			width: 100%;
			height: 138rpx;
			background-color: #fff;
			flex-direction: column;
			align-items: center;
			justify-content: center;
			font-size: 28rpx;

			.font1 {
				margin-left: -520rpx;
				font-size: 26rpx;
				color: #9b9b9b;
			}
		}
	}

	.section {
		height: 180rpx;
		width: 100%;
		display: flex;
		align-items: center;
		margin-top: -20rpx;

		.section-s {
			background: #fff;
			width: 100%;
			height: 138rpx;
			font-size: 28rpx;

			.section-s1 {
				font-size: 26rpx;
				color: #9b9b9b;
				float: left;
				margin-left: 30rpx;
				margin-top: 20rpx;
			}

			.section-s2 {
				font-size: 26rpx;
				margin-top: 20rpx;
				float: right;
				margin-right: 30rpx;
			}

			.section-s3 {
				display: block;
				height: 100%;
				width: 100%;
				text-align: center;
				line-height: 138rpx;
			}
		}
	}
</style>
