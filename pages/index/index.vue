<template>
	<view class="">
		<mycomponent title="hi" content="content..." @tap1="tap"></mycomponent>
	</view>
</template>

<script>
	import uniNumberBox from "@/components/uni-number-box/uni-number-box.vue"
	import mycomponent  from "@/components/mycomponent.vue"
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
		components:{uniNumberBox,
		mycomponent}
	}
</script>

<style lang="less">
@import "../../less.less";
</style>
