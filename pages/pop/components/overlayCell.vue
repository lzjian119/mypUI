<template>
	<view class="cf">
		<view class="cf-bg">
			<image src="https://cdn.img.wenhairu.com/images/2020/05/23/YOrYg.jpg" class="cf-bg-cover" mode="aspectFill"></image>
		</view>
		<view class="cf-title-bg">
			<image class="cf-title-bg-cover" src="https://cdn.img.wenhairu.com/images/2020/05/23/YO2sj.png" mode="aspectFit"></image>
		</view>
		<view class="cf-title">
			<text class="cf-title-text">Overlay</text>
			<image class="cf-title-hint" src="https://cdn.img.wenhairu.com/images/2020/05/23/YOvLH.png" mode="aspectFit"></image>
		</view>
		<view class="cf-left">
			<image src="https://cdn.img.wenhairu.com/images/2020/05/23/YObjv.png" class="cf-left-bg" mode="aspectFit"></image>
		</view>
		<view class="cf-body">
			<view class="cf-item">
				<view class="cf-item-bg">
					<image src="https://cdn.img.wenhairu.com/images/2020/05/23/YOL8o.png" class="cf-item-bg-cover" mode="aspectFit"></image>
				</view>
				<view class="cf-item-tl">
					<image src="https://cdn.img.wenhairu.com/images/2020/05/23/YTC4D.png" class="cf-item-tl-bg" mode="aspectFit"></image>
				</view>
				<view class="cf-item-br">
					<image src="https://cdn.img.wenhairu.com/images/2020/05/23/YOzX3.png" class="cf-item-br-bg" mode="aspectFit"></image>
				</view>
				<view class="cf-item-title">
					<text class="cf-item-title-text" v-for="(item,idx) in ['是','通','用']" :key="idx">{{item}}</text>
				</view>
			</view>
			<view class="cf-item">
				<view class="cf-item-bg">
					<image src="https://cdn.img.wenhairu.com/images/2020/05/23/YOL8o.png" class="cf-item-bg-cover" mode="aspectFit"></image>
				</view>
				<view class="cf-item-tl">
					<image src="https://cdn.img.wenhairu.com/images/2020/05/23/YTC4D.png" class="cf-item-tl-bg" mode="aspectFit"></image>
				</view>
				<view class="cf-item-br">
					<image src="https://cdn.img.wenhairu.com/images/2020/05/23/YOzX3.png" class="cf-item-br-bg" mode="aspectFit"></image>
				</view>
				<view class="cf-item-title">
					<text class="cf-item-title-text" v-for="(item,idx) in ['自','关','闭']" :key="idx">{{item}}</text>
				</view>
			</view>
			<view class="cf-item">
				<view class="cf-item-bg">
					<image src="https://cdn.img.wenhairu.com/images/2020/05/23/YOL8o.png" class="cf-item-bg-cover" mode="aspectFit"></image>
				</view>
				<view class="cf-item-tl">
					<image src="https://cdn.img.wenhairu.com/images/2020/05/23/YTC4D.png" class="cf-item-tl-bg" mode="aspectFit"></image>
				</view>
				<view class="cf-item-br">
					<image src="https://cdn.img.wenhairu.com/images/2020/05/23/YOzX3.png" class="cf-item-br-bg" mode="aspectFit"></image>
				</view>
				<view class="cf-item-title">
					<text class="cf-item-title-text" v-for="(item,idx) in ['设','背','景']" :key="idx">{{item}}</text>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		
	}
</script>

<style lang="scss" scoped>
	.cf {
		position: relative;
		width: 750rpx;
		height: 422rpx;
		overflow: hidden;
		
		&-bg {
			width: 750rpx;
			height: 422rpx;
			overflow: hidden;
			
			&-cover {
				width: 750rpx;
				height: 422rpx;
			}
		}
		&-title {
			position: absolute;
			flex-direction: row;
			align-items: center;
			left: 375rpx;
			top: 30rpx;
			transform: translateX(-50%);
			
			&-bg {
				position: absolute;
				left: 375rpx;
				top: 20rpx;
				transform: translateX(-50%);
				
				&-cover {
					width: 260rpx;
					height: 130rpx;
				}
			}
			&-text {
				font-size: 52rpx;
				line-height: 80rpx;
				color: #FFFFFF;
			}
			&-hint {
				width: 70rpx;
				height: 100rpx;
			}
		}
		&-body {
			position: absolute;
			right: 25rpx;
			width: 540rpx;
			top: 140rpx;
			flex-direction: row;
			justify-content: space-between;
		}
		&-item {
			position: relative;
			
			&-bg {
				&-cover {
					width: 150rpx;
					height: 274rpx;
				}
			}
			&-tl {
				position: absolute;
				top: 0;
				left: 0;
				
				&-bg{
					width: 60rpx;
					height: 57rpx;
				}
			}
			&-br {
				position: absolute;
				right: 0;
				bottom: 0;
				
				&-bg {
					width: 60rpx;
					height: 57rpx;
				}
			}
			&-title {
				position: absolute;
				width: 150rpx;
				height: 274rpx;
				left: 0;
				top: 0;
				flex-direction: column;
				justify-content: center;
				align-items: center;
				
				&-text {
					font-size: 48rpx;
					font-weight: 600;
					color: #729aa1;
					line-height: 66rpx;
				}
			}
		}
		&-left {
			position: absolute;
			bottom: 0;
			left: 0;
			
			&-bg {
				width: 320rpx;
				height: 320rpx;
			}
		}
	}
</style>
