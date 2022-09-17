<template>
	<view>
		<!-- 顶部区域 -->
		<view class="smart-page-head">
			<view class="smart-page-head-title">audio音频组件</view>
		</view>
		<view class="smart-padding-warp">
			<audio style="text-align: left;" :src="current.src" :poster="current.poster" :name="current.name" :author="current.author" controls="true"></audio>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				current:{
					poster:'https://bjetxgzv.cdn.bspapp.com/VKCEYUGU-uni-app-doc/7fbf26a0-4f4a-11eb-b680-7980c8a877b8.png',
					name:'致爱丽丝',
					author:'贝多芬',
					src:'https://bjetxgzv.cdn.bspapp.com/VKCEYUGU-hello-uniapp/2cc220e0-c27a-11ea-9dfb-6da8e309e0d8.mp3',
				},
			}
		},
		onLoad:function(event){
			console.log('页面加载完毕');
		},
		onShow:function(event){
			console.log('页面显示完毕');
		},
		onReady:function(event){
			console.log('页面渲染完毕');
		},
		onHide:function(event){
			console.log('页面隐藏');
		},
		methods: {
			
		}
	}
</script>

<style>

</style>
