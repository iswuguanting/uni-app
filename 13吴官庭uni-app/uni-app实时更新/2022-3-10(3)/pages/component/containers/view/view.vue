<template>
	<view>
		<view class="smalt_page_head"><view class="smalt_page_head_title">view</view></view>
		<!-- 主题部分 -->
		<view class="smalt_padding_wrap"><view>flex-direction:row 横向布局</view></view>
		<view class="smalt_flex smalt_row">
			<view class="smalt_item smalt_bg_blue">A</view>
			<view class="smalt_item smalt_bg_green">B</view>
			<view class="smalt_item smalt_bg_red">C</view>
		</view>
		<view><view>flex-direction:row 众向布局</view></view>
		<view class="smalt_flex smalt_column">
			<view class="flex_item_100 smalt_bg_blue">A</view>
			<view class="flex_item_100 smalt_bg_green">B</view>
			<view class="flex_item_100 smalt_bg_red">C</view>
		</view>

		<view>其他布局</view>
		<view>
			<view class="text">纵向布局-自动宽度</view>
			<view class="text text_first_one">纵向布局-固定宽度</view>
			<view class="smalt_flex smalt_row">
				<view class="text">横向布局-自动宽度</view>
				<view class="text">横向布局-自动宽度</view>
			</view>
			<view class="smalt_flex smalt_row text_first_two">
				<view class="text">横向布局-居中</view>
				<view class="text">横向布局-居中</view>
			</view>
			<view class="smalt_flex smalt_row text_first_three">
				<view class="text">横向布局-居右</view>
				<view class="text">横向布局-居右</view>
			</view>
			<view class="smalt_flex smalt_row ">
				<view class="text text_secound_one">横向布局-平均分布</view>
				<view class="text text_secound_two">横向布局-平均分布</view>
			</view>
			<view class="smalt_flex smalt_row text_first_four">
				<view class="text">横向布局-两端对齐</view>
				<view class="text">横向布局-两端对齐</view>
			</view>
			<view class="smalt_flex smalt_row ">
				<view class="text text_secound_three">固定宽度</view>
				<view class="text text_secound_four">自动占满</view>
			</view>
			<view class="smalt_flex smalt_row ">
				<view class="text text_secound_three">固定宽度</view>
				<view class="text text_secound_four">自动占满</view>
				<view class="text text_secound_three">固定宽度</view>
			</view >
			<view class="smalt_flex smalt_row text_first_five" id="app">
				<view class="text text_three_one">一行显示不全的wrap执行</view>
				<view class="text text_three_two">一行显示不全的wrap执行</view>
				<view class="text text_three_three">一行显示不全的wrap执行</view>
			</view>
		</view>
	</view>
	
	
</template>

<script>
export default {
	
	data() {
		
		return {
			
		};
	},
	methods: {}
};
</script>

<style></style>
