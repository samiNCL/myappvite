<template>
	<label :for="name"> {{name}}  </label>

 <input 
 type="text"
  :id="name"
   :style="{width,height}"
   @input="input"
    

   >
</template>


<script type="text/javascript">
 export default{
 	props:{
			name:{type:String},
			width:{type:String},
			height:{type:String},
			value:{type:String}

 },
 	methods:{
 		input(e){
 			var x= e.target.value;
 		}
 	}
}
	
</script>


<style scoped type="text/css">
	
 
</style>

