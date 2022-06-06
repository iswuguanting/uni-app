<template>
	<view>
		<view class="smalt_page_head">
			<view class="smalt_page_head_title">checkbox 多选框按钮</view>
		</view>
		<view class="smalt_padding_wrap">
			<view class="item">
				<checkbox checked="true">
					选中
				</checkbox>
				<checkbox>
					未选中
				</checkbox>
			</view>
			<view class="item">
				<checkbox checked="true" color="#F0AD4E" class="item_first">
					选中
				</checkbox>
				<checkbox color="#F0AD4E" class="item_first">
					未选中
				</checkbox>
			</view>
			<view class="item_today">
				<hr />
			</view>

			推荐展示样式：
			<checkbox-group>
				<label class="list">
					<view>
						<checkbox></checkbox>
						中国
					</view>
				</label>
				<label class="list">
					<view>
						<checkbox></checkbox>
						日本
					</view>
				</label>
				<label class="list">
					<view>
						<checkbox></checkbox>
						美国
					</view>
				</label>
			</checkbox-group>

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
