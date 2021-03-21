<template>
	<view>
			<h1 class="pink" @tap="tap1">{{title}}</h1>
			<div>{{content}}</div>
	</view>
</template>

<script>
	
	export default{
		props:{
			title:{
				type:String,
				default:""
			},
			content:{
				type:String,
				default:""
			}
		},
		methods:{
			tap1:function(){
				console.log(1);
				this.$emit("tap1",this.title)
			}
		}
	}
</script>

<style>
	.pink{color:pink}
</style>
