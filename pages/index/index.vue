<template>
	<view class="">
		<mycomponent title="hi" content="content..." @tap1="tap"></mycomponent>
		<row content="大家好，我是吴枫，很高兴又和你见面了。"></row>
	</view>
</template>

<script>
	import uniNumberBox from "@/components/uni-number-box/uni-number-box.vue"
	import mycomponent  from "@/components/mycomponent.vue"
	import row from "@/components/row.vue"
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
			row
					}
		
	}
</script>

<style lang="less">
@import "../../less.less";
</style>
