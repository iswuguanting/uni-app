<template>
	<view>
		<view class="smalt_page_head">
			<view class="smalt_page_head_title"> scroll-view区域滚动视图</view>
		</view>
		<view class="smalt_padding_wrap">
			<view class="smart_text">可滚动视图区域</view>
			<view> vertical scroll 纵向滚动</view>
			<view>
				<scroll-view class="scroll_y" scroll-y="true">
					<view class="srcoll_view_item smalt_bg_red">A</view>
					<view class="srcoll_view_item smalt_bg_blue">B</view>
					<view class="srcoll_view_item smalt_bg_green">C</view>
				</scroll-view>
			</view>
			<view> vertical scroll 横向滚动</view>
			<view>
				<scroll-view class="scroll_x" scroll-x="true" scroll-left="120">
					<view class="srcoll_view_item_h smalt_bg_red">A</view>
					<view class="srcoll_view_item_h smalt_bg_blue">B</view>
					<view class="srcoll_view_item_h smalt_bg_green">C</view>
				</scroll-view>
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

</style>
