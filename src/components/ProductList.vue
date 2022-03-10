
<template>
<div>
<v-card v-for="(item,index) in array" :key="index">
 
    <v-img
      height="250"
      :src="item.image"
    ></v-img>

    <v-card-title>{{item.title}}</v-card-title>

    <v-card-text>
      <v-row
        align="center"
        class="mx-0"
      >
        <v-rating
          :value="4.5"
          color="amber"
          dense
          half-increments
          readonly
          size="14"
        ></v-rating>

        <div class="grey--text ms-4">
          4.5 (413)
        </div>
      </v-row>

      <div class="my-4 text-subtitle-1">
        $ • Italian, Cafe
      </div>

      <div>Small plates, salads & sandwiches - an intimate setting with 12 indoor seats plus patio seating.</div>
    </v-card-text>

    <v-divider class="mx-4"></v-divider>

    <v-card-title>Tonight's availability</v-card-title>
  </v-card>

</div>
</template>

<script>
//import ItemsList from './productsJSON.vue';
  export default {
    name:'ProductList',
    data: () => ({
      loading: false,
      selection: 1,
      
    }),
    props: ['array']
  }
</script>