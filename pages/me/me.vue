<template>
	<view>
		<view class="display box">
			<view class="">
				<text class="h1">用户名</text><br>
				<text>欢迎您光临四海香！</text>
			</view>
			<view class="">
				<image src="../../static/ICON/14.png" mode="img" class="user"></image>
			</view>
		</view>
		<view class="display justifay box">
			<view class="display justifay">
				<image src="/static/ICON/icon_order.png" mode="" class="icon"></image>
				<text>烹饪历史</text>
			</view>
			<text>></text>
		</view>
		<view class="display justifay box">
			<view class="display justifay">
				<image src="/static/ICON//icon_money.png" mode="" class="icon"></image>
				<text>支付记录</text>
			</view>
			<text>></text>
		</view>
		<view class="display justifay box">
			<view class="display justifay">
				<image src="/static/ICON//icon_msg.png" mode="" class="icon"></image>
				<text>举报投诉</text>
			</view>
			<text>></text>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {

			}
		},
		methods: {

		}
	}
</script>

<style>
	.h1 {
		font-size: 40rpx;
		font-weight: 600;
	}

	.box {
		padding: 40rpx;
		border-bottom: 4px solid #f4f4f4;
	}

	.user {
		width: 100rpx;
		height: 100rpx;
	}

	.icon {
		width: 60rpx;
		height: 60rpx;
		margin-right: 40rpx;
	}

	.justifay {
		align-items: center;
	}

	.display {
		display: flex;
		justify-content: space-between;
	}
</style>