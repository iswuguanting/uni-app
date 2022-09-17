<template>
	<view>
		<view class="smalt_page_head">
			<view class="smalt_page_head_title">buttom 按钮</view>
		</view>
		<view class="smalt_padding_wrap progress_control">
			<button type="primary">页面主操作 normal</button>
			<button type="primary" :loading="true">页面主操作 loading</button>
			<button type="primary" disabled="false">页面主操作 disabled</button>

			<button type="default">页面主操作 normal</button>
			<button type="default" disabled="false">页面主操作 disabled</button>
			<button type="warn">页面警告操作 warn</button>
			<button type="default" disabled="false">页面警告操作 warn</button>

			<button type="primary" plain="true">缕空按钮 plain</button>
			<button type="primary" plain="true" disabled="false">缕空按钮 plain disabled</button>

			<button type="primary" size="mini" class="mini_btn">按钮</button>
			<button type="default" size="mini" class="mini_btn">按钮</button>
			<button type="warn" size="mini" class="mini_btn">按钮</button>

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
