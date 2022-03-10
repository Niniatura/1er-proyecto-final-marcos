<template>
  <v-app>
    <v-main>
      <nav-header></nav-header>
      <form-registro></form-registro>
      <items-list></items-list>
    </v-main>
  </v-app>
</template>

<script>
import FormRegistro from './components/FormRegistro.vue';
import NavHeader from './components/NavHeader.vue';
import ItemsList from './components/Card.vue';

export default {
  name: 'App',

  components: {
    NavHeader,
    FormRegistro,
    ItemsList
  },
};
</script>
