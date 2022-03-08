<template>
  <v-app>
    <v-main>
      <nav-header></nav-header>
      <form-registro></form-registro>
    </v-main>
  </v-app>
</template>

<script>
import FormRegistro from './components/FormRegistro.vue';
import NavHeader from './components/NavHeader.vue'

export default {
  name: 'App',

  components: {
    NavHeader,
    FormRegistro
  },

  data: () => ({
    //
  }),
};
</script>
