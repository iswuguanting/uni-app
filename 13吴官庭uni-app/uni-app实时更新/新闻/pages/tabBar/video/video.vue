<template>
	<view>
		<!-- 第一部分 顶部 -->
		<view class="items">
			<view class="item">
				<view class="item-xs">推荐</view>
				<view class="item-xs">千里眼</view>
				<view class="item-xs">搞笑</view>
				<view class="item-xs">娱乐</view>
				<view class="item-xs">社会</view>
				<view class="item-xs">音乐</view>
				<view class="item-xs">科技</view>
			</view>
		</view>
		
		<!-- 第二部分 1-->
		<view class="sp">
			<navigator url="../videocontent/videocontent">
				<view class="x">600斤的公牛不甘心被杀，宁愿跳进大海之中，结局令人遗憾</view>
			</navigator>
			<video class="y" style="width: 100%; height: 400rpx;" src="https://bjetxgzv.cdn.bspapp.com/VKCEYUGU-uni-app-doc/360e4b20-4f4b-11eb-8a36-ebb87efcf8c0.mp4" @error="videoErrorCallback" ></video>
			<view class="dibu">
				<view class="wenzi">
					<view class="wenzizf">
						<image style="width: 45rpx; height: 45rpx;" 
						src="../../../static/2017090511563086816.jpg"></image>
					</view>
					<view class="wenzizf" style="font-size: 32rpx;">开心哈哈大笑...</view>
					<view class="wenzizf" style="color: #999999; margin-top: 0rpx;">|</view>
					<view class="wenzizf" style="font-size: 32rpx;color: #dd524d; font-weight: bold;">
						关注
					</view>
				</view>
				<view class="tupian">
					<view class="tupiandx">
						<image style="width: 35rpx; height: 35rpx;"
						src="../../../static/xingxi.png"></image>
					</view>
					<view class="tupiandx">
						<image style="width: 35rpx; height: 35rpx;"
						src="../../../static/dianzan.png"></image>
					</view>
					<view class="tupiandx" style="margin-top: -14rpx;padding-right: 20rpx;">...</view>
				</view>
			</view>
		</view>
		
		<view class="sp2">
			<navigator url="../videocontent/videocontent">
				<view class="x">这些箱子里装的中高档卷烟共有1350条，27余万支</view>
			</navigator>
			<video class="y" style="width: 100%; height: 400rpx;" src="https://bjetxgzv.cdn.bspapp.com/VKCEYUGU-uni-app-doc/360e4b20-4f4b-11eb-8a36-ebb87efcf8c0.mp4" @error="videoErrorCallback" ></video>
			<view class="dibu">
				<view class="wenzi">
					<view class="wenzizf">
						<image style="width: 45rpx; height: 45rpx;" 
						src="../../../static/y10.jpg"></image>
					</view>
					<view class="wenzizf" style="font-size: 32rpx;">往事随风飘去...</view>
					<view class="wenzizf" style="color: #999999; margin-top: 0rpx;">|</view>
					<view class="wenzizf" style="font-size: 32rpx;color: #dd524d; font-weight: bold;">
						关注
					</view>
				</view>
				<view class="tupian">
					<view class="tupiandx">
						<image style="width: 35rpx; height: 35rpx;"
						src="../../../static/xingxi.png"></image>
					</view>
					<view class="tupiandx">
						<image style="width: 35rpx; height: 35rpx;"
						src="../../../static/dianzan.png"></image>
					</view>
					<view class="tupiandx" style="margin-top: -14rpx;padding-right: 20rpx;">...</view>
				</view>
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
.items {
		background-color: #ffffff;
		position: fixed;
		/*固定位置设置新闻条的时候用*/
		z-index: 1;
		/*显示层级，设置在最上显示*/
	
		width: 100%;
		top: 90rpx;
		
	}

	.item {
		background-color: #ffffff;
		display: flex;
		/*显示在一行，弹性布局*/
		flex-direction: row;
		/*在一行显示、两个同时用才会显示在一行*/
		margin: 5rpx 10rpx 20rpx 10rpx;
		font-size: 40rpx;
		color: #333333;
		margin-bottom: 20rpx;



	}

	.item-ss {
		width: 100%;
		height: 60rpx;
	}

	/*选项卡*/
	.tab_title view {
		display: inline-block;
		/*一行内显示 没有加.的view表示概括定义在这个文件下的view标签*/
		margin-left: 30rpx;
		line-height: 30rpx;
		/*文字行高*/
		color: #ffffff;

	}

	.dibu {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		-webkit-justify-content: space-between;
		margin-top: 30rpx;
		margin-bottom: 20rpx;
	}

	.wenzi {
		display: flex;
		flex-direction: row;

	}

	.tupian {
		display: flex;
		flex-direction: row;
	}

	.tupiandx {
		margin-left: 60rpx;
	}

	.wenzizf {
		margin-right: 20rpx;
	}

	.x {
		margin-top: 80rpx;
		margin-bottom: 30rpx;
	}

	.item-xs {
		color: #DD524D;
		font-weight: bold;
		/*文字加粗*/
	}

	.a {
		margin-right: 120rpx;
		height: 50rpx;
	}

	.ap image {
		width: 250rpx;
		height: 100rpx;
	}

	.ap {
		border-radius: 10rpx;
		width: 250rpx;
		height: 100rpx;
		overflow: hidden;
		margin: auto;
	}

	.b {}


	.scroll_X {
		height: 50rpx;
		width: 100%;
		white-space: nowrap;
		/*强制在一行内显示所有文本*/
	}

	.item {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		color: #333333;
		background-color: #FFFFFF;
		border-bottom: 1rpx solid #C8C7CC;
	}

	.tab_title {
		/*表示 tab_title下面所有的view都一样显示*/
		display: inline-block;
		/*在一行内显示*/
		margin-left: 10rpx;
		height: 80rpx;
		line-height: 70rpx;
		/*文字行高*/
		color: #333333;
		background-color: #FFFFFF;
		border-bottom: 1rpx solid #C8C7CC;
	}

	.tab-x {
		color: #333333;
		background-color: #FFFFFF;
	}

	.scroll_x {
		height: 60rpx;
		/*设置高度*/
		width: 100%;
		/*设置宽度*/
		white-space: nowrap;
		/*强制在一行内显示所有文本*/
	}

	.gray {
		color: #C8C7CC;
	}

	.gray1 {
		color: #DD524D;
	}

	.hd {
		display: inline-block;
		/*在一行内显示*/
	}

	.tab {
		background-color: #DD524D;
	}

	.shgd {
		position: fixed;
		/*固定位置*/
		position: absolute;
		/*xx固定位置*/
		z-index: 1;
	}

	/*隐藏导航条*/
	scroll-view::-webkit-scrollbar {
		display: none;
		width: 0;
		height: 0;
		color: transparent;
	}

	.sp {
		border-bottom: 1rpx solid #e5eaf3;
		margin: 10rpx 10rpx 20rpx 20rpx;

	}

	.reg-rigth {
		color: #DD524D;
		margin-right: 10rpx;
		padding-left: 10rpx;
	}

	.z {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		margin-bottom: 30rpx;
		margin-top: 20rpx;
		height: 70rpx;
	}

	.zs {
		display: flex;
	}

	.z1 {
		margin-bottom: 10rpx;
		margin-right: 300rpx;
		margin-top: 20rpx;
	}

	.z-h {
		height: 60rpx;
		margin-right: 10rpx;
		display: flex;
		flex-direction: row;
		font-size: 35rpx;
	}

	.z-z {
		font-size: 30rpx;
		color: #C8C7CC;
	}

	.z-z1 {
		font-size: 30rpx;
		color: #C8C7CC;
		margin: 20rpx;
	}

	.z-z2 {
		font-size: 30rpx;
		color: #C8C7CC;
		margin: 20rpx;
	}


	.y {
		margin: 0rpx;
		flex: 1;
		/*自动适应宽度*/
	}
</style>
