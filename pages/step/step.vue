<template>
	<view class="max">
		<view class="display card_top">
			<view class="display justifay">
				<image src="/static/ICON/icon_cha.png" mode="aspectFit" class="icon"></image>
				<text>已收藏9个行程</text>
			</view>
			<view class="display justifay">
				<image src="/static/ICON//92.png" mode="aspectFit" class="icon"></image>
				<text>历史</text>
			</view>
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

<style lang="less">
	.display {
		display: flex;
	}

	.justifay {
		justify-content: center;
	}

	.icon {
		width: 40rpx;
		height: 40rpx;
	}

	.max {
		.card_top {
			justify-content: space-between;
			padding: 30rpx;

			text {
				margin-left: 20rpx;
			}
		}
	}
</style>