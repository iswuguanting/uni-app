<template>
	<view>
		<view class="smalt_page_head">
			<view class="smalt_page_head_title">slider 滑块</view>
		</view>
		
		<view class="smalt_padding_wrap">
			<view class="uni_title">显示当前value</view>
			<view>
				<slider value="50" @change="sliderChange" show-value='true'></slider>
			</view>
			
			<view class="uni_title">设置步进step跳动</view>
			<view>
				<slider value="60" @change="sliderChange" step="5" show-value='true'></slider>
			</view>
			
			<view class="uni_title">设置最小值/最大值</view>
			<view>
				<slider value="100" @change="sliderChange" min="50" max="200" show-value=""></slider>
			</view>
			
			<view class="uni_title">不同颜色的大小的模块</view>
			<view>
				<slider value="50" @change="sliderChange" activeColor="#ffcc33" backgroundColor="#000000" block-color="#8a6de9" block-size="20"></slider>
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
			sliderChange(e){
				console.log('value 发生变化：' + e.detail.value)
			}
		}
	}
</script>

<style>

</style>
