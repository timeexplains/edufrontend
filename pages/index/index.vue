<template>
	<view class="">
		<!-- <mycomponent title="hi" content="content..." @tap1="tap"></mycomponent> -->
<div class="lecture-container">
<div class="view-container">
<div class="view-main">
	<div class="top-panel">
<div class="reader forceUseInfiniteWrapper" style="scroll-behavior: auto;">
	<div class="wrap">
		<row content="大家好，我是吴枫，很高兴又和你见面了。"></row>
		<row content="现在，请将屏幕调整成全屏，与我沉浸在Python的魔法世界。【windows系统：请按F11（或Fn+F11)；mac系统：请同时按control+command+F。】"></row>
		<row content="在上一关，我们已经推开了Python世界的大门，通过Python中最基本的print()函数，开启了我们第一声问候。现在，我们先回顾下上一关的知识点。"></row>
		<imageRow imgPath="../static/knowlg.jpg"></imageRow>
		<row content="凯文.凯利以预测科技发展趋势而出名，在90年代里，他曾在他的著作《失控》中提及了云计算、物联网、虚拟现实等概念。他预言人类的未来是镜像世界。"></row>
		<row content="奇异博士利用魔法制造了镜像世界进行战斗，减少对现实世界的破坏；我们人类用代码程序也创造了一个镜像世界，在镜像世界里面高效地解决现实世界里的繁琐任务。"></row>
		<row content="其实呀，python世界可以看作部分现实世界的【镜像】，部分现实世界的东西、概念都可在python世界里找到对应，比如：现实世界中最常见的数字，文字，符号在Python世界就是：【数据】。"></row>
		<row content="不同类型的数据呀，『长相』不一样，各司其职。只有认清各类型数据的『长相』，了解它们的功能，才能在镜像世界里完成现实世界的任务。"></row>
		<imageRow imgPath="../static/pyworld.png"></imageRow>
	</div>
	</div>
	</div>
	<div class="bottom-panel">
		<div class="progress-bar-container progress-bar">
		<div class="progress-bar" style="width: 14%;"></div>
		</div>
		<div class="next-button clickable next-button button-pointer">
			<i class="icon iconfont icon-enter-" style="font-size: 34px;"></i>
		</div>
	</div>
</div>
</div>
</div>
	</view>
</template>

<script>
	import uniNumberBox from "@/components/uni-number-box/uni-number-box.vue"
	import mycomponent  from "@/components/mycomponent.vue"
	import row from "@/components/row.vue"
	import imageRow from "@/components/image-row.vue"
	export default {
		data() {
			return {
				title: 'hello...'
			}
		},
		onLoad() {

		},
		methods: {
			tap:function(e){
					console.log(e);
				}
		},
		components:{
			uniNumberBox,
			mycomponent,
			row,
			imageRow
		}
		
	}
</script>

<style lang="less">
@import "../../less.less";
</style>
