<template>
	<!-- 17 -->
	<view>
		<!-- top部分 -->
		<view class="inform">
			<view class="inform-s" v-for="(item,index) in items" @tap="tabChange(index)" :class="activeIndex==index?'active':''">
				<text>{{item.m}}</text>
				<text>{{item.x}}</text>
			</view>
		</view>
		<view :class="activeIndex==0?'':'none'">
			<view class="message" v-for="(massage,index) in massage" :key="massage.id">
				<text>{{massage.time}}</text>
				<text class="fonts">{{massage.fonts}}</text>
			</view>
		</view>
		<view :class="activeIndex==1?'':'none'">
			<view @tap="systemMessage" class="message" v-for="(system,index) in system" :key="system.id">
				<text>{{system.time}}</text>
				<text>{{system.system}}</text>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				activeIndex: 0,
				items: [{
						m: '短消息'
					},
					{
						x: '系统通知'
					}
				],
				system:[
					{
						id: '0',
						time: "2019-10-05 22:39:45",
						system:'系统消息系统消息系统消息系统消息系统消息系统消息...',
					},
					{
						id: '1',
						time: "2019-10-05 22:39:45",
						system:'系统消息系统消息系统消息系统消息系统消息系统消息...',
					}
				],
				massage: [{
						id: '0',
						time: "2019-10-05 22:39:45",
						fonts: '消息内容消息内容消息内容消息内容消息内容消息...'
					},
					{
						id: '1',
						time: "2019-10-05 22:39:45",
						fonts: '消息内容消息内容消息内容消息内容消息内容消息...'
					},
					{
						id: '2',
						time: "2019-10-05 22:39:45",
						fonts: '消息内容消息内容消息内容消息内容消息内容消息...'
					},
					{
						id: '3',
						time: "2019-10-05 22:39:45",
						fonts: '消息内容消息内容消息内容消息内容消息内容消息...'
					}
				]
			};
		},
		methods: {
			tabChange(index) {
				this.activeIndex = index;
				console.log(index)
			},
			systemMessage(){
				uni.navigateTo({
					url:'systemT'
				})
			}
		}
	}
</script>

<style lang="scss">
	// 1
	.inform {
		height: 100rpx;
		width: 100%;
		background-color: #efeef3;
		display: flex;
		color: #b5b4b9;

		.inform-s {
			line-height: 100rpx;
			text-align: center;
			width: 50%;
			font-size: 30rpx;
		}

	}

	// 点击是那条线
	.active {
		box-sizing: border-box;
		border-bottom: 4rpx solid #eb303b;
		color: #eb303b;
	}


	// 2
	.message {
		height: 150rpx;
		width: 92%;
		display: flex;
		margin-left: 30rpx;
		justify-content: center;
		flex-wrap: wrap;
		flex-direction: column;
		border-bottom: 1rpx solid #f5f5f5;

		text {
			width: 100%;
			display: flex;
			font-size: 26rpx;
			color: #b5b4b9;
		}

		.fonts {
			margin-top: 20rpx;
		}
	}
	.none{
		display: none;
	}
</style>
