<template>
	<view class="max">
		<view class="display card_top">
			<view class="display justifay">
				<image src="/static/ICON/icon_cha.png" mode="aspectFit" class="icon"></image>
				<text>已收藏12个餐宴</text>
			</view>
			<view class="display justifay">
				<image src="/static/ICON//icon_clear.png" mode="aspectFit" class="icon"></image>
				<text>清空</text>
			</view>
		</view>
		<image src="../../static/ICON/goods3.jpg" mode="aspectFit" class="card_img"></image>
		<view class="card_end display ">
			<view>
				<text>盛夏海鲜家宴</text><br>
				<text>已收藏12个餐宴</text>
			</view>
			<view class="center">
				<image src="/static/ICON//icon_clear.png" mode="aspectFit" class="icon"></image><br>
				<text>清空</text>
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

		.card_img {
			width: 94%;
			display: block;
			margin: 0 auto;
			border-top-left-radius: 20rpx;
			border-top-right-radius: 20rpx;
		}

		.card_end {
			justify-content: space-between;
			padding: 30rpx;

			.center {
				text-align: center;
			}
		}
	}
</style>