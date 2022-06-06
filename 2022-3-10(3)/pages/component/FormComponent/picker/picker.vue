<template>
	<view>
		<view class="smalt_page_head">
			<view class="smalt_page_head_title">{{ title }}</view>
		</view>
		<view class="smalt_padding_wrap">
			<view class="uni_title">普通选着器</view>
			<view class="uni_list">
				<view class="uni_lis_cell">
					<view class="uni_lis_cell_left">当前选择</view>
					<view class="uni_lis_cell_db">
						<picker @change="bindPickerChange" :range="array" :value="index" range-key="name">
							<view class="uni_input">{{array[index].name}}</view>
						</picker>
					</view>
				</view>
			</view>
			<view class="uni_title uni_commmon_pl">日期选择器</view>
			<view class="uni_list">
				<view class="uni_lis_cell">
					<view class="uni_lis_cell_left">当前选择</view>
					<view class="uni_lis_cell_db">
						<picker mode="date" :value="date" :start="startDete" :end="endDate" @change="bindDateChange">
							<view class="uni_input">{{date}}</view>
						</picker>
					</view>
				</view>
			</view>
			<view class="uni_title uni_commmon_pl">时间选择器</view>
			<view class="uni_list">
				<view class="uni_lis_cell">
					<view class="uni_lis_cell_left">当前选择</view>
					<view class="uni_lis_cell_db">
						<picker mode="time" :value="time" start="09:01" end="21.01" @change="bindTimeChange">
							<view class="uni_input">{{time}}</view>
						</picker>
					</view>
				</view>
			</view>
		</view>
	</view>
</template>
<script>
	function getDate(type) {
		const date = new Date();

		let year = date.getFullYear();
		let month = date.getMonth() + 1;
		let day = date.getDate();

		if (type === 'start') {
			year = year - 60;
		} else if (type === 'end') {
			year = year + 2
		}
		month = month > 9 ? month : '0' + month
		day = day > 9 ? day : '0' + day

		return `${year} - ${month} - ${day}`;
	}
	export default {
		data() {
			return {
				title: 'picker,选择列表',
				array: [{
					name: '中国'
				}, {
					name: '美国'
				}, {
					name: '日本'
				}, {
					name: '巴西'
				}],
				index: 0,
				date: getDate({
					format: true
				}),
				startDete: getDate('start'),
				endDate: getDate('end'),
				time: '12.01'
			}
		},
		methods: {
			bindPickerChange: function(e) {
				this.index = e.detail.value;
			},
			bindDateChange: function(e) {
				this.date = e.detail.value;
			},
			bindTimeChange: function(e) {
				this.time = e.detail.value;
			}
		}
	}
</script>
<style>

</style>
