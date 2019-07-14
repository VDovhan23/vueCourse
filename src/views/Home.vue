<template>
  <div >
    <!-- <AppButton  
    @click.prevent="clickk"
    >
       КУРВА
      </AppButton> -->

      <AppInput
        name="email"
      >
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
  methods: {
    clickk() {
      console.log('clickk');
      
    }
  },

   
}
</script>
