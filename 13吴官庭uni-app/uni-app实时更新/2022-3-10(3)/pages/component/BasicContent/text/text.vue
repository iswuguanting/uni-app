<template>
	<view>
		<view class="smalt_page_head">
			<view class="smalt_page_head_title">text 文本组件</view>
		</view>
		<view class="smalt_padding_wrap">
			<view class="text_box">
				<text>{{text}}</text>
			</view>
			<button type="primary" :disabled="!canAdd" @click="add">添加一行</button>
			<button type="warn" :disabled="!canRemove" @click="remove">移除一行</button>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				texts:[
					'1.HBuilder,400万开发者选择的IDE',
					'2.HBuilderX,轻巧.极速,极客编辑器',
					'3.uni-app,终极跨平台方案',
					'4.HBuilder,400万开发者选择的IDE',
					'5.HBuilderX,轻巧.极速,极客编辑器',
					'6.uni-app,终极跨平台方案',
					'7.HBuilder,400万开发者选择的IDE',
					'8.HBuilderX,轻巧.极速,极客编辑器',
					'9.uni-app,终极跨平台方案',
					'10. .....'
				],
				text:'',
				canAdd:true,
				canRemove:false,
				extraLine:[]
			}
		},
		methods: {
			add:function(e){
				this.extraLine.push(this.texts[this.extraLine.length % 12]);
				// console.log(this.extraLine);
				this.text = this.extraLine.join('\n');
				this.canAdd = this.extraLine.length < 20;
				this.canRemove = this.extraLine.length > 0;
			},
			remove:function(){
				if(this.extraLine.length > 0){
					this.extraLine.pop();
					this.text = this.extraLine.join('\n');
					this.canAdd = this.extraLine.length < 20;
					this.canRemove = this.extraLine.length > 0;
				}
			}
			
		}
	}
</script>

<style>

</style>
