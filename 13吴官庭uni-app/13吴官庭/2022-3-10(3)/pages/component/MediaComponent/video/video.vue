<template>
	<view>
		<view class="smalt_page_head">
			<view class="smalt_page_head_title">video 视频组件</view>
		</view>
		<view class="smalt_padding_wrap">
			<video
			  id="myVideo"
			  :danmu-list="danmuList"
			  enable-danmu="true"
			  danmu-btn="true"
			  src="https://bjetxgzv.cdn.bspapp.com/VKCEYUGU-uni-app-doc/360e4b20-4f4b-11eb-8a36-ebb87efcf8c0.mp4"
			  >
			  </video>
		</view>
		<view class="btn_s">
			<input v-model="danmuValue" class="smart_input" type="text" placeholder="在此处输入弹幕内容"/>
		</view>
		<view class="btn_v">
			<button @click="sendDanmu" class="page_body_buttom">发送弹幕</button>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
			    danmuList:[
					{
						text: '第 1s 出现的弹幕',
						color: '#ff0000',
						time: 1
					},
					{
						text: '第 3s 出现的弹幕',
						color: '#ff00ff',
						time: 3
					}
				],
				danmuValue:''
			}
		},
		onReady: function (res) {
			this.videoContext = uni.createVideoContext('myVideo');
			setTimeout(()=>{
				//this.showVideo = true
			},350);
			
			//this.showVideo = true
		},
		methods: {
			sendDanmu:function(e){
				this.videoContext.sendDanmu({
					text:this.danmuValue,
					color:'red'
				});
				this.danmuValue='';
			}
		}
	}
</script>

<style>
video{
	width: 100%;
}
.btn_v{
	margin: 15rpx;
}
.btn_s{
	
	height: 100rpx;
	font-size: 30rpx;
	margin:0 30rpx 0 30rpx;
	border: 1rpx solid #C8C7CC;
	border-radius:10rpx;
}
</style>
