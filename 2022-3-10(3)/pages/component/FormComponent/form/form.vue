<template>
	<view>
		<view class="smalt_page_head">
			<view class="smalt_page_head_title">form 表单</view>
		</view>
		<view class="container">
			<form @submit="formSubmit" @reset="formReset">
				<view class="formitem uni_column">
					<view class="formtitle">switch</view>
					<view>
						<switch name='switch'></switch>
					</view>
				</view>
				<view class="formitem uni_column">
					<view class="formtitle">radio</view>
					<radio-group name='radio'>
						<label>
							<radio value="radio1"/><text>选项一</text>
						</label>
						<label>
							<radio value="radio2"/><text>选项二</text>
						</label>
					</radio-group>
				</view>
				<view class="formitem uni_column">
					<view class="formtitle">checkbox</view>
					<checkbox-group name='checkbox'>
						<label>
							<checkbox value="checkbox1"/><text>选项一</text>
						</label>
						<label>
							<checkbox value="checkbox2"/><text>选项二</text>
						</label>
					</checkbox-group>
				</view>
				<view class="formitem uni_column">
					<view class="formtitle">slider</view>
					<slider value="50" name='slider' show-value></slider>
				</view>
				<view class="formitem uni_column">
					<view class="formtitle">input</view>
					<input class="uni_input" name='input' placeholder="这是一个输入框" />
				</view>
				<view >
					   <button form-type="submit">提交</button>
					   <button type="default" form-type="reset">重置</button>
				</view>
			</form>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				submit:''
			}
		},
		methods: {
			formSubmit: function(e){
				var formdata = e.detail.value
				console.log('form发生了submit事件,携带数据为：'+JSON.stringify(formdata))
				uni.showModal({
					content:'表单数据内容：'+JSON.stringify(formdata),
					showCancel:false
				})
			},
			formReset: function(e){
				console.log('清空数据')
				uni.showModal({
					content:'清空数据',
					showCancel:false
				})
			}
		}
	}
</script>

<style>

</style>
