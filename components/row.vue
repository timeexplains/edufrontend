<template>
	<div class="resourceContainer">
		<div class="iconWrap">
			<img src="../static/teacher.png" alt="icon">
		</div>
		<div class="splitLine"></div>
		<div class="content">
			<div class="resource-title"></div>
						<div class="chat">
<section class="plugin-markdown">

	<div class="plugin-markdown-chat">
		<div>
			<p>
				{{content}}
			</p>
		</div>
	</div>
</section>
</div>
	</div>
	</div>
</template>

<script>
	export default {
		props:{
			content:{
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
		    display: -webkit-box;
		    display: -webkit-flex;
		    display: -ms-flexbox;
		    display: flex;
		    width: 100%;
		    line-height: 2;
		    color: #c2c1c6;
		    -webkit-box-sizing: content-box;
		    box-sizing: content-box;
			margin-bottom:40px;
	}
	.resource-title{
		position: absolute;
		left:0;
		top:-28px;
		height:20px;
		line-height: 20px;
		color:#201f26;
		font-size:14px;
		font-weight:700;
	}
	.iconWrap{
		margin-right: 10px;
		width:30px;
		height:30px;
		flex-grow: 0;
	}
	.iconWrap img{
		display: block;
		width:30px;
		height:30px;
		border-radius: 50%;
	}
	.splitLine{
		width:2px;	
		margin-right:16px;
		border-radius: 1px;
		flex-grow: 0;
		background-color: rgba(255, 203, 124, 0.3)
	}
	.chat{
		max-width:1076px;
		word-break:break-all;
		font-size:0;
	}
	.content{
		width:calc(100%-62px);
		font-size:16px;
		position:relative;
	}
	.plugin-markdown{
		display:inline-block;
		width:100%;
		height:100%;
		font-size:16px;
		word-break:break-word;
		overflow: hidden;
	}
</style>
