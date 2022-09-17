<template>
	<view>
		<view class="smalt_page_head">
			<view class="smalt_page_head_title">switch 开关</view>
		</view>
		<view class="smalt_padding_wrap">
			<view class="uni_title">默认样式</view>
			<view>
				<switch checked @change='switch1Change'></switch>
				<switch @change='switch2Change'></switch>
			</view>
			<view class="uni_title">不同颜色和尺寸的switch</view>
			<view>
				<switch checked color="#ffcc33" class="item_first"></switch>
				<switch color="#ffcc33" class="item_first"></switch>
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
			switch1Change: function(e){
				console.log('switch1 发生 change 事件，携带值为',e.detail.value)
			},
			switch2Change: function(e){
				console.log('switch2 发生 change 事件，携带值为',e.detail.value)
			}
		}
	}
</script>

<style>

</style>
