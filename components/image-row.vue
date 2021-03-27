<template>
	<div class="resourceContainer">
		<div class="iconWrap">
		</div>
		<div class="splitLine"></div>
<div class="content">
		<img v-bind:src='imgPath' alt="icon2">
</div>
	</div>
</template>

<script>
	export default {
		name: "imageRow",
		props:{
			 imgPath:{
			 	type:String,
			 	default:""
			 }
		},
		onLoad() {
	
		},
		methods: {
		}
	}
	
</script>

<style>
	.resourceContainer{
		 position: relative;
		 display: flex;
		 width: 100%;
		 line-height:2;
		 color:#c2c1c6;
		 box-sizing: content-box;
		 /* background:rgba(194,193,198,.1); */
		 padding:20px 0px 0px 0px;
	}
	
	.iconWrap{
		margin-right: 10px;
		width:30px;
		height:30px;
		flex-grow: 0;
	}
	
	.splitLine{
		width:2px;	
		margin-right:16px;
		border-radius: 1px;
		flex-grow: 0;
		background-color: rgba(255, 203, 124, 0.3)
	}
	
	.content{
		    max-width: 640px;
		    min-height: 136px;
		    border-radius: 4px;
		font-size:16px;
		position:relative;
	}
	
	.content img{
		width: 100%;
		height: auto;
		border-radius: 4px;
	}
	
</style>
