<template>
  <div >

      {{form}}

      <AppInput
        name="email"
        type="text"
        v-model="form.email"
      >
      inp
     
      </AppInput>

  </div>
</template>

<script>
// @ is an alias to /src

import AppButton from '@/components/AppButton';
import AppInput from '@/components/AppInput';

export default {
  name: 'home',
  components: {
    AppButton, AppInput
  },
  data() {
    return {
      form: {
        email: ''
      }
    }
  },
  methods: {
    clickk() {
      console.log('clickk');
      
    }
  },

   
}
</script>
