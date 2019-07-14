<template>
  <div class="container">
    <router-link
      class="btn btn-danger"
      @click.native="$emit('click', $event)"
      :to="{to}"
      
    >
      <slot/>
    </router-link>
  </div>
</template>


<script>
export default {
  data() {
    return {
      
    };
  },
  props: {
   to:{
     required: false,
     type: Object
   }
  }
};
</script>

<style>
</style>
