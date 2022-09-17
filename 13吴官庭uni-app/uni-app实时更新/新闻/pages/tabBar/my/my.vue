<template>
	<view>
		<view class="dd">
			<view class="item1">
				<image class="tx" style="width: 130rpx; height: 130rpx;" src="../../../static/mmao.png"></image>
				<view class="item2">
					<view class="item3">HI--欢迎回来</view>
					<view class="item4"><text class="itemz">登录</text></view>
				</view>
			</view>

			<view class="er1">
				<view class="er2">关注3</view>
				<view class="er3">|</view>
				<view class="er4">话题0</view>
			</view>
		</view>
		
		<view class="item-dj">
			<view>
				<navigator url="../topic/topic">
					<view class="item-left">
						<image class="menpiao" src="../../../static/shouzh.png"></image>
					</view>
					<view class="item-left">收藏</view>
				</navigator>
			</view>
			<view>
				<navigator url="../topic/topic">
					<view class="item-left">
						<image class="menpiao1" src="../../../static/lishi.png"></image>
					</view>
					<view class="item-left">历史</view>
				</navigator>
			</view>
			<view>
				<navigator url="../topic/topic">
					<view class="item-left">
						<image class="menpiao1" src="../../../static/shezhi.png"></image>
					</view>
					<view class="item-left">设置</view>
				</navigator>
			</view>
		</view>
		
		<view>
			<image style="width: 100%; height: 90rpx;" src="../../../static/gg.jpg"></image>
		</view>
		
		<view class="button">
			<image class="buttons" style="width: 100%;height: 300rpx;" src="../../../static/stup.png"></image>
			<view class="button">
				<text class="hh">已有</text>385,893<text class="hh">人</text>
				<br/>
				<text class="hh">在这里发布身边的新鲜事</text>
				<view class="reg-right">我也要发布</view>
				<view><text class="hh">先去逛逛</text><image style="width: 38rpx;height: 38rpx;" src="../../../static/you.png"></image></view>
			</view>
		</view>
	</view>
</template>

<script>
export default {
	data() {
		return {};
	},
	methods: {}
};
</script>

<style scoped>
.dd {
	padding-bottom: 0rpx;
	background-image: url(../../../static/bjmh.png);
	/*添加图片*/
	background-position: center;
	margin-top: -30rpx;
	height: 280rpx;
}

.tx {
	margin-top: 10rpx;
}

.item1 {
	display: flex;
	margin-top: 30rpx;
	margin-left: 20rpx;
}

.item2 {
	margin-top: 15rpx;
}

.item3 {
	margin-left: 20rpx;
	color: #ffffff;
	font-weight: bold;
	margin-top: 10rpx;
}

.item4 {
	border-radius: 20rpx;
	color: #ffffff;
	width: 150rpx;
	heigh: 100rpx;
	background-color: #dd524d;
	margin-left: 40rpx;
	margin-top: 10rpx;
}

.itemz {
	color: #ffffff;
	margin-left: 45rpx;
}

.er1 {
	display: flex;
	margin-top: 80rpx;
	margin-left: 80rpx;
	opacity: 0.8;
}

.er2 {
	margin-left: 50rpx;
	color: #ffffff;
}

.er3 {
	margin-left: 140rpx;
	color: #ffffff;
}

.er4 {
	margin-left: 150rpx;
	color: #ffffff;
}
.e {
	-webkit-flex: 1;
	flex: 1;
}

.smart {
}

.item-dj {
	display: flex;
	flex-direction: row;
	-webkit-flex: 1;
	flex: 1;

	border-bottom: 1rpx solid #e6e6e6;
	margin-top: -50rpx;
	margin-bottom: 5rpx;
}

.item-left {
	height: 10rpx;
	line-height: 71rpx;
	/*设置行高和标签高度一致，实现 垂直居中*/
	width: 50%;
	/*水平居中*/
	text-align: center;
	margin: 90rpx;
	font-size: 20rpx;
	padding-bottom: 1rpx;
	margin-top: 20rpx;
}

.menpiao {
	width: 45rpx;
	height: 45rpx;
	text-align: center;
	margin-top: 70rpx;
}

.menpiao1 {
	width: 45rpx;
	height: 45rpx;
	text-align: center;
	margin-top: 70rpx;
}

.menpiao2 {
	width: 40rpx;
	height: 40rpx;
	text-align: center;
	margin-top: 70rpx;
}

.buttons {
	margin-top: 12rpx;
}

.button {
	text-align: center;
}

.reg-right {
	border: 1rpx solid #dd524d;
	width: 250rpx;
	height: 65rpx;
	text-align: center;
	color: #dd524d;
	border-radius: 40rpx;
	margin-bottom: 20rpx;
	line-height: 70rpx;
	margin-top: 40rpx;
	/*上外间距*/
	margin-left: 240rpx;
}

.buttonx {
	color: #999999;
}

.hh {
	color: #999999;
}

.zh {
	height: 200rpx;
}
</style>
