<template>
	
	
<div v-if="type == 2" class="resourceContainer2">
			<div class="iconWrap">
			</div>
			<div class="splitLine"></div>
	<div class="content">
			<img v-bind:src='imgPath' alt="icon2">
	</div>
</div>
		
<div  class="resourceContainer" v-else>
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
		name: "rowAdapter",
		props:{
			 imgPath:{
			 	type:String,
			 	default:""
			 },
			 content:{
				 type:String,
				 default:""
			 },
			 type:{
				 type:Number,
				 default:0
				}
		},
		onLoad() {
	
		},
		methods: {
		}
	}
		
</script>

<style>
@import "../row-image.less";
@import "../row.less";

</style>
