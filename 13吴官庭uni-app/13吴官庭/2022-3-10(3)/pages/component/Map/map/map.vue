<template>
	<view>
		<view class="smalt_page_head">
			<view class="smalt_page_head_title">map 地图</view>
		</view>
		
		<view class="smalt_padding_wrap">
			<map class="map" :latitude="21.220500" :longitude="110.398900" :markers="covers"></map>
		</view>
		
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				covers:[
					{
						latitude:21.220500,
						longitude:110.398900,
						iconpth:'../../static/230.png'
					},
					
				]
			}
		},
		methods: {
			
		}
	}
</script>

<style>
	.smalt_padding_wrap{
		margin-bottom: 30rpx;
	}
.map{
	width: 100%;
	height: 600rpx;
}
</style>
