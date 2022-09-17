<template>
	<view>
		<!-- 顶部标题 -->
		<view class="items">
			<view class="item">
				<navigator url="../pursue/pursue">
					<view class="item-x">追踪</view>
				</navigator>
				<navigator url="../topic1/topic1">
					<view class="item-x"><text class="item-xx">话题榜</text></view>
				</navigator>
				<navigator url="../oppinions/oppinions">
					<view class="item-x">观点榜</view>
				</navigator>
				<image class="item-y" style="width: 35rpx; height: 35rpx;" 
				src="../../../static/shousuo.png"></image>
			</view>
		</view>
		
		<view class="bt"></view>
		<!-- 话题 -->
		<view class="ht">
			<view>
				<image class="a" src="../../../static/t1.png"></image>
			</view>
			<view class="hts">
				<view><text class="item-xx">曼联客场不败场次在英超排名第二，阿森纳27次客场不败</text></view>
				<view class="c">曼联客场对阵阿斯顿维拉，这场比赛的结果对于现阶段
				曼联客场对阵阿斯顿维拉，这场比赛的结果对于现阶段曼联客场对阵阿斯顿维拉，这场比赛的结果对于现阶段
				曼联客场对阵阿斯顿维拉，这场比赛的结果对于现阶段曼联客场对阵阿斯顿维拉，这场比赛的结果对于现阶段</view>
				<view class="d">
					<view class="hotimage">
						<image class="img1" src="../../../static/y10.jpg"></image>
						<image class="img2" src="../../../static/y3.jpg"></image>
						<image class="img3" src="../../../static/y6.jpg"></image>
						<image class="img4" src="../../../static/y5.jpg"></image>
					</view>
					<view class="hotimage-x">119观点</view>
				</view>
			</view>
		</view>
		
		<!-- 话题2 -->
		<view class="ht">
			<view>
				<image class="a" src="../../../static/t2.png"></image>
			</view>
			<view class="hts">
				<view><text class="item-xx">#司机为救婴儿闯红灯#</text></view>
				<view class="c">曼联客场对阵阿斯顿维拉，这场比赛的结果对于现阶段
				曼联客场对阵阿斯顿维拉，这场比赛的结果对于现阶段曼联客场对阵阿斯顿维拉，这场比赛的结果对于现阶段
				曼联客场对阵阿斯顿维拉，这场比赛的结果对于现阶段曼联客场对阵阿斯顿维拉，这场比赛的结果对于现阶段</view>
				<view class="d">
					<view class="hotimage">
						<image class="img1" src="../../../static/y4.jpg"></image>
						<image class="img2" src="../../../static/y2.jpg"></image>
						<image class="img3" src="../../../static/y8.jpg"></image>
						<image class="img4" src="../../../static/y8.jpg"></image>
					</view>
					<view class="hotimage-x">1419观点</view>
					<view class="hotimage-y">热</view>
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
.hotimage {
		margin-right: 120rpx;

	}

	.hotimage-x {
		margin-left: 30rpx;
		margin-right: 15rpx;
		font-size: 25rpx;
	}

  

	.hotimage image {
		width: 30rpx;
		height: 30rpx;
		position: absolute;

	}

	.hotimage .img1 {
		left: 20rpx;
	}

	.hotimage .img2 {
		left: 50rpx;
	}

	.hotimage .img3 {
		left: 80rpx;
	}

	.hotimage .img4 {
		left: 110rpx;
	}

	.hotimage .imgs {
		margin-left: 1000rpx;
	}

	.hotimage .img6 {
		margin-right: 700rpx;
	}

	.items {
		position: fixed;
		z-index: 1;
		background-color: #FFFFFF;
		width: 100%;


	}

	.bt {
		width: 100rpx;
		height: 70rpx;

	}

	.item {
		display: flex;
		/*显示在一行，弹性布局*/
		flex-direction: row;
		/*在一行显示、两个同时用才会显示在一行*/
		margin: 5rpx 10rpx 20rpx 10rpx;
		font-size: 40rpx;
		color: #333333;
		background-color: #FFFFFF;

	}

	.item-x {
		margin-right: 45rpx;

	}

	.item-y {
		margin-top: 10rpx;
		margin-left: 180rpx;
	}

	.hotimage-y {
		border: 1rpx solid #DD524D;
		width: 30rpx;
		text-align: center;
		color: #DD524D;
		border-radius: 10rpx;
		font-size: 17rpx;
		height: 32rpx;

	}

	.item-xx {
		font-weight: bold;
		/*文字体重加粗*/

	}


	.ht {
		border-bottom: 1rpx solid #CCD0D9;
		margin-bottom: -12rpx;

	}

	.checkbox-item {
		color: #DD524D;
		width: 20rpx;
		height: 20rpx;
	}

	.hts {
		margin-left: 20rpx;
	}

	.c {
		margin-top: 13rpx;
	}

	.a {
		width: 30rpx;
		height: 30rpx;
		margin-top: 13rpx;
	}

	.d {
		margin-bottom: 40rpx;
		display: flex;
		flex-direction: row;
		white-space: nowrap;
		margin-top: 30rpx;
	}
</style>
