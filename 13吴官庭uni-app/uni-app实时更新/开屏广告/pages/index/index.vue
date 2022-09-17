<template>
	<view class="content">
		<view style="ad">
			<swiper style="width: 100%;" :style="{height:windowHeight}" indicator-dots="true" autoplay="true" interval="3000">
				<swiper-item class="ad1"></swiper-item>
				<swiper-item class="ad2"></swiper-item>
				<swiper-item class="ad3"></swiper-item>
			</swiper>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				windowHeight:'200px'
			}
		},
		onLoad() {
			this.windowHeight=uni.getSystemInfoSync().windowHeight+"px";
			console.log(this.windowHeight);
		},
		methods: {

		}
	}
</script>

<style>
	.ad1{
		margin: 0;
		padding: 0;
		background-repeat: no-repeat;
		background-size: 100% 100%;
		background-attachment: fixed;
		background-image: url(../../static/1.png);
	}
	.ad2{
		margin: 0;
		padding: 0;
		background-repeat: no-repeat;
		background-size: 100% 100%;
		background-attachment: fixed;
		background-image: url(../../static/2.png);
	}
	.ad3{
		margin: 0;
		padding: 0;
		background-repeat: no-repeat;
		background-size: 100% 100%;
		background-attachment: fixed;
		background-image: url(../../static/3.png);
	}
	.content{
		position: relative;
	}
	.ad{
		position: absolute;left: 30px;top: 30px;
	}
</style>
