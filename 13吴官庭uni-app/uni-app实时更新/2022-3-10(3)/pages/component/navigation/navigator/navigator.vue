<template>
	<view>
		<view class="smalt_page_head">
			<view class="smalt_page_head_title">navigator 导航</view>
		</view>
		<view class="smalt_padding_wrap">
			<navigator url="../newpage/newpage" hover-class="navigator">
				<button type="default">跳转到新页面</button>
			</navigator>
		
		<navigator url="../newpage/newpage?title=redirect" open-type="redirect" hover-class="other-navigator-hover">
			<button type="default">在当前页面打开</button>
		</navigator>
		<navigator url="../../../taBar/api/api" open-type="switchTab" hover-class="other-navigator-hover">
			<button type="default">跳转到Tab页面</button>
		</navigator>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title:'navigator'
			}
		},
		methods: {
			
		}
	}
</script>

<style>

</style>
