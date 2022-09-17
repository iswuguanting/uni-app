<template>
	<view>
	<view class="tab">
		<view class="tab_title">
			<scroll-view scroll-x="true" class="scroll_x">
				<view>
					<image style="width: 30rpx; height: 35rpx;" src="../../../static/shouhu.png"></image>
				</view>
				<view>要闻</view>
				<view>推荐</view>
				<view>关注流</view>
				<view>24小时</view>
				<view>娱乐</view>
				<view>桂林</view>
				<view>财经</view>
				<view>生活</view>
				<view>科技</view>
				<view>军事</view>
				<view>体育</view>
				<view>汽修</view>
				<view>健康</view>
				<view>国际</view>
				<view>千里眼</view>
				<view>5G</view>
			</scroll-view>
		</view>
	</view>	
	<view class="three">
		<view class="three-s">为您更新了15条内容</view>
	</view>
	<view class="twos">
		<view class="twoss">
			4℃ 小雨 桂林 PM2.5
		</view>
		<view class="left">
			<input type="text" style="width: 180rpx; margin-right: 20rpx;font-size: 25rpx;"
			placeholder="搜索关键词" class="search_input"/>
		</view>
	</view>
	<view class="d-three">
		<view class="xw-three">
			<view> 2020,我们温暖的记忆</view>
		<view class="threes">
			<view class="j"><text class="zd">置顶</text></view>
			<view class="j">新闻联播</view>
			<view class="j">45评</view>
		</view>
		</view>
		
		<view class="xw-three">
			<view> 森林大县57年无大火是怎样做到的</view>
		<view class="threes">
			<view class="j"><text class="zd">置顶</text></view>
			<view class="j">光明网</view>
			<view class="j">17评</view>
		</view>
		</view>
		
	</view>
	<navigator url="../../newsinfo/newsinfo">
		<view class="d-three">
			<view class="d-threes">
				<view>
					<image style="width: 200rpx;height: 160rpx;"
					src="../../../static/d.png"></image>
				</view>
				<view class="d-threess">几年近疯狂，涉案金额超3亿，一个背包客牵出全国跨省倒烟大案</view>
			</view>
			<view> 
			<view class="threess">大河网 38评</view>
			</view>
		</view>
	</navigator>
	<view class="d-three">
		<view class="d-threes">
			<view>
				<image style="width: 200rpx;height: 160rpx;"
				src="../../../static/xw10.png"></image>
			</view>
			<view class="d-threess">中国老年化水平加速，论养老保险在中国的重要性？人们应不应该买保险？</view>
		</view>
		<view >
			<view class="threess">新京报官微  58评</view>
		</view>
	</view>
	<view class="d-three">
		<view class="d-threes">
			<view>
			<image style="width: 200rpx;height: 160rpx;"
			src="../../../static/b.png"></image>
			</view>
			<view>
				<view class="d-threess">人们都喜欢聚在一起，人们聚在一起是好是坏</view>
			</view>
		</view>
		<view>
			<view class="threess">烽火君 18评</view>
		</view>
	</view>
	<view class="d-three">
		<view> 加微信交友群，喜欢就聊，找喜欢的人</view>
		<view class="d-threes">
			<view class="a">
				<image style="width: 200rpx;height: 160rpx;"
				src="../../../static/b.png"></image>
			</view>
			<view class="a">
				<image style="width: 200rpx;height: 160rpx;"
				src="../../../static/c.png"></image>
			</view>
			<view class="a">
				<image style="width: 200rpx;height: 160rpx;"
				src="../../../static/f.png"></image>
			</view>
		</view>
		<view>
			<view class="threess">广告 我主良缘文化</view>
		</view>
	</view>
	<view class="d-three">
		<view class="d-threes">
			<view>
			<image style="width: 200rpx;height: 160rpx;"
			src="../../../static/f.png"></image>
			</view>
			<view>
				<view class="d-threess">随着经济的发展，中国各个城市发展速度越来越快，经济发展迅速
				，人们幸福快乐</view>
			</view>
		</view>
		<view>
			<view class="threess">时代发展 8评</view>
		</view>
	</view>
	
	<view class="d-three">
		<view class="d-threes">
			<view>
			<image style="width: 200rpx;height: 160rpx;"
			src="../../../static/c.png"></image>
			</view>
			<view>
				<view class="d-threess">随着经济的发展，中国各个城市发展速度越来越快，经济发展迅速
				，人们幸福快乐</view>
			</view>
		</view>
		<view>
			<view class="threess">时代发展 8评</view>
		</view>
	</view>
	<view class="d-three">
		<view class="d-threes">
			<view>
			<image style="width: 200rpx;height: 160rpx;"
			src="../../../static/1.png"></image>
			</view>
			<view>
				<view class="d-threess">随着经济的发展，中国各个城市发展速度越来越快，经济发展迅速
				，人们幸福快乐</view>
			</view>
		</view>
		<view>
			<view class="threess">时代发展 3评</view>
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
	scroll-view ::-webkit-scrollbar {
		display: none !important;
		width: 0 !important;
		height: 0 !important;
		-webkit-appearance: none;
		background: transparent;
	} /* 去除滚动条 */
.search{
	display: flex;
	flex-direction: row;
}
.two{
	margin: 0rpx 40rpx 25rpx 30rpx;
	color: #ffffff;
	margin-top: 30rpx;
	display: flex;
	flex-direction: row;
}
.twos{
	color: #ffffff;
	display: flex;
	background-color: #dd524d;
	margin-top: -10rpx;
	width: 100%;
	justify-content: space-between;
	-webkit-justify-content:space-between;
	height: 70rpx;
}
.twoss{
	margin-left: 20rpx;
}
.reds{
	color: #dd524d;
	height: 40rpx;
}
.xw-three{}
.three{
	width: 100%;
	height: 120rpx;
	background-color: #dd524d;
}
.three-s{
	color: #ffffff;
}
.d-three{
	border-bottom: 1rpx solid #ccd0d9;
	margin: 20rpx 20rpx 20rpx 20rpx;
}
.d-threes{
	display: flex;
	flex-direction: row;
}

.a{
	margin: 20rpx 10rpx 10rpx 20rpx;
}
.d-threess{
	margin-left: 30rpx;
	
}
.threes{
	display: flex;
	flex-direction: row;
	margin: 5rpx 10rpx 10rpx 10rpx;
	font-size: 25rpx;
	color: #808080;
}
.j{
	margin-right: 25rpx;
}
.threess{
	margin-bottom: 20rpx;
	font-size: 25rpx;
	color: #808080;
}
.search .left{
	flex: 1;
	-webkit-flex:1;
	margin-right: 70rpx;
	height: 10rpx;
}
.search .right{
	width: 120rpx;
}
.search_input{
	background-color: #f8f8f8;
	border-radius: 40rpx;
	padding: 5rpx 30rpx 6rpx 30rpx;
	margin-right: 1rpx;
}
.search_img{
	height: 48rpx;
	width: 48rpx;
}
.tab_title view{
	display: inline-block;
	margin-left: 30rpx;
	height: 80rpx;
	line-height: 80rpx;
	color: #ffffff;
}
.tab{
	background-color: #dd524d;
	height: 100rpx;
	position: fixed;
	z-index: 1;
	left: 0;
	right: 0;
	width: 100%;
	margin-top: 0rpx;
}
.zd{
	color: #dd524d;
}
.scroll_x{
	height: 60rpx;
	width: 100%;
	white-space: nowrap;
}
scroll-view::-webkit-scrollbar{
	display: none;
	width: 0;
	height: 0;
	color: transparent;
}
.news_list{
	margin: 200rpx 25rpx 25rpx 25rpx;
	position: absolute;
	padding-bottom: calc(var(--window-bottom));
	width: 100%;
}
.news_item{
	height: 150rpx;
	border-bottom: 1rpx solid #c8c7cc;
	display: flex;
	flex-direction: row;
	margin-bottom: 20rpx;
}
.news_list image{
	width: 180rpx;
	height: 140rpx;
	margin-right: 30rpx;
}
.news_list .title{
	font-size: 35rpx;
}
.news_list .time{
	color: #c0c0c0;
	font-size: 30rpx;
	margin-top: 15rpx;
}
</style>
