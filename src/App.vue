
<template>
	<div class="container">

	
	<!--  The props is property in the tag-->
	<form> 
		<c-input

	name="Question to Twitter" 
	width="15em"
	height='2em'
	/>
<c-button 
v-on:click="greet"
text= "Post it"
color=""
width="5em"
height='2em'
:disabled="var1"

/> 
<!--  
<button v-on:click="greet" >Click</button>
 -->
	</form>
	<!-- Here HTML -->
	<input width="3em"  v-model="test.name" />  is <input width="3em" v-model="test.Age" /> 
<br>

 {{test.name}}  is  {{test.Age}} years old.

</div>
</template>


<script type="text/javascript">

	import CButton from "./components/CButton.vue" //We bring component
	import CInput from "./components/CInput.vue" //We bring component 2


	export default{
		components:{
			CButton,
			CInput
		},

		data(){
			return {

				var1:false,
				test:{
					name:"Mohammad",
					Age:"45"
				}
			}
		},
		methods:{
			greet(){
				alert("Hi, I will go Twitter")
			}
		}
	}


 
</script>


<style scoped type="text/css">
	
	/* Here CSS*/
	@import 'https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css'

</style>


