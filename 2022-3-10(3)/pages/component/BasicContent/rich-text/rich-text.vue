<template>
	<view>
		<view class="smalt_page_head"><view class="smalt_page_head_title">rich-text,富文本</view></view>
		<view class="smalt_padding_wrap">
			<view><rich-text :nodes="nodes"></rich-text></view>
			<view><rich-text :nodes="strings"></rich-text></view>
		</view>
	</view>
</template>

<script>
export default {
	data() {
		return {
			nodes: [
				{
					name: 'div',
					attrs: {
						class: 'div-class',
						style: 'line-height:60px;color:red;text-align:center;background-color:#09BB07'
					},
					children: [
						{
							type: 'text',
							text: 'Hello&nbsp;uni-app!'
						}
					]
				}
			],
			strings: '<div style="text-align:center;margin-top:50rpx;"><img src="/static/logo.png"/></div>'
		};
	},
	methods: {}
};
</script>

<style></style>
