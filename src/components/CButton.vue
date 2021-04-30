<template>
	<!-- {{text is in props, to accept parameter from App.vue}} -->
	<button
	
	:style="{color, height}"  
	:disabled="disabled"
	>
	{{text}}
	</button> 
</template>


<script type="text/javascript">
	export default{

		props:{
			text:{type:String,required:true},
			color : {type:String},
			disabled:{type:Boolean},
			width:{type:String},
			height:{type:String}


		}// properties for this components 
	}
</script>


<style scoped type="text/css">
	
	/* Here CSS*/
</style>


