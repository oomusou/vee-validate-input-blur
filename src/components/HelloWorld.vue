<template>
  <div class="hello">
    <div>
      <div>
        <input v-validate="'required|email'" name="email1" type="text">
      </div>
      <div>
        <input v-validate="'required|email'" name="email2" type="text">
      </div>
      <div>
        <span>{{ errors.first('email1') }}</span>
        <span>{{ errors.first('email2') }}</span>
      </div>
    </div>
  </div>
</template>

<script>
import Vue from 'vue';
import VeeValidate from 'vee-validate';

Vue.use(VeeValidate);

export default {
  name: 'HelloWorld',
};
</script>
