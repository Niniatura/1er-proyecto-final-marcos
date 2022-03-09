<template>
  <v-app>
    <v-main>
      <nav-header></nav-header>
      <form-registro></form-registro>
      <product-list></product-list>
    </v-main>
  </v-app>
</template>

<script>
import FormRegistro from './components/FormRegistro.vue';
import NavHeader from './components/NavHeader.vue';
import ProductList from './components/ProductList.vue'

export default {
  name: 'App',

  components: {
    NavHeader,
    FormRegistro,
    ProductList
  },

  data: () => ({
    //
  }),
};
</script>
