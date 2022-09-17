<template>
	<view>
		<view class="smalt_page_head">
			<view class="smalt_page_head_title"> swiper 滑块视图</view>
		</view>
		<view class="smalt_padding_wrap">
			<swiper circular :indicator-dots="indicatorDots" :autoplay="autoplay" :interval="interval" :duration="duration">
				<swiper-item><view class="swiper_item smalt_bg_blue">A</view></swiper-item>
				<swiper-item><view class="swiper_item smalt_bg_green">B</view></swiper-item>
				<swiper-item><view class="swiper_item smalt_bg_red">C</view></swiper-item>
				<swiper-item><view class="swiper_item smalt_bg_red">d</view></swiper-item>
			</swiper>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				indicatorDots:true,
				autoplay:true,
				// 多少时间滑动
				interval:500,  
				// 滑动的速度多快
				duration:500
			}
		},
		methods: {
			
		}
	}
</script>

<style>

</style>
