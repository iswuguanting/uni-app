<template>
	<view>
		<view class="smalt_page_head">
			<view class="smalt_page_head_title">progress,进度</view>
		</view>
		<view class="smalt_padding_wrap">
			<view class="progress_box">
				<progress :percent="pgList[0]" show-info="true" stroke-width="3" activeColor="blue" active="true"><!-- active 加了慢慢移动 -->
					
				</progress>
			</view>
			<view class="progress_box">
				<progress :percent="pgList[1]" show-info="true" activeColor="skyblue" stroke-width="3">
					
				</progress>
			</view>
			
			<view class="progress_control">
				<button type="primary" @click="setProgress">设置进度</button>
				<button type="warn" @click="clearProgress">清除进度</button>
				
			</view>
			<view class="progress_box_schoe"></view>
			<view class="progress_control">
				<progress :percent="hfList[0]" show-info="true" stroke-width="3" active="true">
					
				</progress>
				
			</view>
			<view class="progress_control">
				<button type="primary" @click="playProgress">设置进度</button>
				<button type="warn" @click="outProgress">清除进度</button>
			</view>
			
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				pgList:[0, 0],
				hfList:[0, 0]
			}
		},
		methods: {
			setProgress(){
				this.pgList=[20, 40];
			},
			clearProgress(){
				this.pgList=[0, 0];
			},
			playProgress(){
				this.hfList=[90];
			},
			outProgress(){
				this.hfList=[0];
			}
		}
	}
</script>

<style>

</style>
