<template>
  <v-app>
    <v-main>
      <nav-header></nav-header>
      <form-registro></form-registro>
      <single-card></single-card>
      
    </v-main>
  </v-app>
</template>

<script>
import FormRegistro from './components/FormRegistro.vue';
import NavHeader from './components/NavHeader.vue';
//import ProductList from './components/ProductList.vue';
import SingleCard from './components/SingleCard.vue'

export default {
  name: 'App',

  components: {
    NavHeader,
    FormRegistro,
    SingleCard
  },
};
</script>
