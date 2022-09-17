<template>
	<view>
		<view class="smalt_page_head">
			<view class="smalt_page_head_title">image 图片</view>
		</view>
		<view class="smalt_padding_wrap">
			<view>
				示例1
				<text>\n本地图片</text>
			</view>
			<view class="smart_center" style="background: #FFFFFF; font-size: 0;">
				<image class="image" mode="widthFix" src="../../../../static/logo.png"></image>
			</view>
			<view>
				示例2
				<text>\n网络图片</text>
			</view>
			<view class="smart_center" style="background: #FFFFFF; font-size: 0;">
				<image class="image" mode="widthFix" src="https://img0.baidu.com/it/u=985192759,2265250910&fm=253&fmt=auto&app=138&f=JPEG?w=500&h=333"></image>
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

<style>
.smart_center{
	text-align: center;
}
.image{
	margin: 40rpx 0;
	width: 300rpx;
}
</style>
