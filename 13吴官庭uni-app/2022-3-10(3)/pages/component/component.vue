<template>
	<view>
		<view class="smalt">uni-app</view>
		
		
		<view class="smalt_first">1.容器</view>
		<view class="smalt_twore" @click="Containers('view')"><text>view视图</text></view>
		<view class="smalt_twore_onlione" @click="Containers('scroll-text')"><text>scroll.view滚动视图</text></view>
		<view class="smalt_twore_onlitwo" @click="Containers('swiper')"><text>swiper可滑动视图</text></view>
		
		<view class="smalt_first">2.基础内容</view>
		<view class="smalt_twore" @click="Basic_content('text')"><text>文本编辑</text></view>
		<view class="smalt_twore_onlione" @click="Basic_content('rich-text')"><text>rich-text富文本编辑</text></view>
		<view class="smalt_twore_onlitwo" @click="Basic_content('progress')"><text>progress进度条</text></view>
		
		<view class="smalt_first">3.表单组件</view>
		<view class="smalt_twore" @click="Form_Component('buttom')"><text>buttom 按钮</text></view>
		<view class="smalt_twore" @click="Form_Component('radio')"><text>radio 按钮</text></view>
		<view class="smalt_twore" @click="Form_Component('checkbox')"><text>checkbox 多选框</text></view>
		<view class="smalt_twore" @click="Form_Component('input')"><text>input 输入控件</text></view>
		<view class="smalt_twore" @click="Form_Component('picker')"><text>picker 选择列表</text></view>
		<view class="smalt_twore" @click="Form_Component('slider')"><text>slider 模块</text></view>
		<view class="smalt_twore" @click="Form_Component('switch')"><text>switch 开关</text></view>
		<view class="smalt_twore" @click="Form_Component('textarea')"><text>textarea 多行文本输入框</text></view>
		<view class="smalt_twore" @click="Form_Component('form')"><text>form 表单</text></view>
		
		<view class="smalt_first">4.导航</view>
		<view class="smalt_twore" @click="Navigation('navigator')"><text>navigator 导航</text></view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			Containers(e){       //  这是超链接
				if(typeof e==='string'){      
					uni.navigateTo({
						url:'containers/'+e+'/'+e,
					});
				}
				else{
					uni:navigateTo({
						url:e.url
					})
				}
			},
			Basic_content(e){       //  这是超链接
				if(typeof e==='string'){      
					uni.navigateTo({
						url:'BasicContent/'+e+'/'+e,
					});
				}
				else{
					uni:navigateTo({
						url:e.url
					})
				}
			},
			Form_Component(e){       //  这是超链接
				if(typeof e==='string'){      
					uni.navigateTo({
						url:'FormComponent/'+e+'/'+e,
					});
				}
				else{
					uni:navigateTo({
						url:e.url
					})
				}
			},
			Navigation(e){       //  这是超链接
				if(typeof e==='string'){      
					uni.navigateTo({
						url:'navigation/'+e+'/'+e,
					});
				}
				else{
					uni:navigateTo({
						url:e.url
					})
				}
				console.log(e.url)
			}
		}
	}
</script>

<style>


</style>
