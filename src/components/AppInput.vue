<template>
<div>
  <input 
  :type="inputType" 
	  :name="name"
	  :id="name"
	  class="form-control"
	  @input="$emit('input', $event.target.value)"
	  />
  <a 
   @click.prevent="passwordShow = !passwordShow"
   href="" 
   v-if="type=='password'"
   >{{passwordShow? 'Hide ' : 'Show ' }} password</a>
   
</div>
</template>


<script>
export default {
  data() {
	return {
	  passwordShow: false,
	};
  },
  computed: {
	  inputType() {
		return  this.passwordShow ? 'text' : this.type
	  }
  },
  props: {
	type: {
	  required: false,
	  type: String,
	  default: "text"
	},
	name: {
	  required: false,
	  type: String,
	  default: "email"
	}
  }
};
</script>

<style>
</style>
