<template>
  <input 
    type="text" 
    name="email" 
    id="email" 
    class="form-control"
  >
</template>


<script>
export default { 
  data() {
    return {
      
    };
  },
  props: {
      name: {
          required: true,
          type: String
      },
      name: {     
        required: false,     
        type: String,
        default: 'email'
      }
  }
};
</script>

<style>
</style>
