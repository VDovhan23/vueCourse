<template>
  <div>
    {{form}}
    <AppInput name="email" type="text" placeholder="bla bla" ></AppInput>
  </div> 
</template>

<script>
// @ is an alias to /src

import AppButton from "@/components/AppButton";
import AppInput from "@/components/AppInput";

export default {
  name: "home",
  components: {
    AppButton,
    AppInput
  },
  data() {
    return {
      form: {
        email: "waselews1@gmail.com"
      }
    };
  },
  methods: {
    clickk() {
      console.log("clickk");
    }
  }
};
</script>
