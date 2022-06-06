<template>
	<view>
		<view class="smalt_page_head">
			<view class="smalt_page_head_title">{{title}}</view>
		</view>
		<view class="smalt_padding_wrap">
			<view class="item">可自动获取焦点的</view>
			<view>
				<input class="smalt_input" focus="true" placeholder="自动获取焦点" />
			</view>
			<view>右下角显示搜索</view>
			<view>
				<input class="smalt_input" confirm-type="search" placeholder="右下角显示搜索" />
			</view>
			<view>控制最大长度输入</view>
			<view>
				<input class="smalt_input" maxlength="10" placeholder="控制最大长度输入" />
			</view>
			<view>
				同步获取输入值
				<br />
				<text class="inputgrout">{{inputValue}}</text>
			</view>
			<view>
				<input class="smalt_input" @input="onKeyInput" placeholder="同步获取输入值" />
			</view>
			<view>数字输入</view>
			<view>
				<input class="smalt_input" type="number" placeholder="这是一个数字输入框" />
			</view>
			<view>密码输入</view>
			<view>
				<input class="smalt_input" type="text" placeholder="这是一个密码输入框" />
			</view>
			<view>带小数点输入</view>
			<view>
				<input class="smalt_input" type="digit" placeholder="这是一个带小数点输入框" />
			</view>
			<view>身份证输入</view>
			<view>
				<input class="smalt_input" type="idcard" placeholder="这是一个身份证输入框" />
			</view>
			<view>带清除按钮</view>
			<view class="wrapper">
				<input class="smalt_input" :value="clearinputValue" @input="clearInput" placeholder="这是一个带清除按钮的输入框" />
				<text v-if="showClearIcon" @click="clearIcon" class="uni_icon"></text>
			</view>
			<view>可查看密码的输入框</view>
			<view class="wrapper">
				<input class="smalt_input" placeholder="请输入密码" :password="showPassword" />
				<text class="uni_icon" :class="[!showPassword ? 'eye_active' : '']" @click="changPassword">
					&#xe568
				</text>
			</view>
		</view>
	</view>
</template>
<script>
	export default {
		data() {
			return {
				title: 'input输入框',
				inputValue: '',
				showPassword: '',
				clearinputValue: '',
				showClearIcon: false

			}
		},
		methods: {
			onKeyInput: function(event) {
				this.inputValue = event.detail.value;
			},
			clearInput: function(event) {
				this.clearinputValue = event.detail.value;
				if (event.detail.value.length > 0) this.showClearIcon = true;
			},
			clearIcon: function(event) {
				this.clearinputValue = '';
				this.showClearIcon = false;
			},
			changPassword: function(event) {
				this.showPassword = !this.showPassword;
			}
		}
	}
</script>
<style>
</style>
