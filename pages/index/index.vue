<template>
	<view class="max">
		<view class="">
			<image src="@/static/ICON/banner.png" mode="aspectFit" class="banner"></image>
		</view>
		<view class="nr">
			<view class="icon">
				<view class="">
					<image src="@/static/ICON/5.png" mode="aspectFit"></image><br>
					<text>餐宴</text>
				</view>
				<view class="">
					<image src="@/static/ICON/7.png" mode="aspectFit"></image><br>
					<text>名厨</text>
				</view>
				<view class="">
					<image src="@/static/ICON/4.png" mode="aspectFit"></image><br>
					<text>坝坝宴</text>
				</view>
				<view class="">
					<image src="@/static/ICON/6.png" mode="aspectFit"></image><br>
					<text>餐饮周边</text>
				</view>
			</view>
			<image src="@/static/ICON/8.png" mode="aspectFit" class="banner"></image>
		</view>
		<view class="mc">
			<image src="@/static/ICON/9.png" mode="aspectFit" class="mc_man"></image>
			<text>更多名厨</text>
		</view>
		<view class="mc">
			<image src="@/static/ICON/10.png" mode="aspectFit" class="mc_man"></image>
			<view class="">

			</view>
			<text>更多餐宴</text>
		</view>
		<image src="@/static/ICON/gg.jpg" mode="aspectFit" class="banner"></image>

	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		created() {
			this.getNav()
		},
		onLoad() {

		},
		methods: {
			getNav() {
				uni.request({
					url: 'http: //api.brqc.com.cn/cpz/shxmp/navlist',
					data: {},
					success: (res) => {
						console.log(res);
						this.menu = res.data.data
					},
					error: (err) => {
						console.log(err)
					}
				})
			}
		}
	}
</script>

<style lang="less">
	.max {
		background-color: #f4f4f4;
		width: 100%;

		// position: relative;
		.banner {
			width: 100%;
			height: 380rpx;
			background-color: white;
		}

		.serch {
			width: 80%;
			padding: 20rpx;
			margin: -40rpx auto 0;
			border: 1px solid red;
			height: 40rpx;
			text-align: center;
			box-sizing: border-box;
			position: absolute;
		}

		.nr {
			background-color: white;
			margin: 0rpx;

			.icon {
				margin: 0 6%;
				display: flex;
				justify-content: space-between;
				text-align: center;

				&>view {
					width: 20%;

					image {
						width: 100%;
						height: 160rpx;
					}
				}
			}
		}

		.mc {
			background-color: white;
			margin-top: 20rpx;
			text-align: center;

			.mc_man {
				width: 90%;
				height: 100rpx;
				display: block;
				margin: 0 auto;
			}
		}
	}
</style>