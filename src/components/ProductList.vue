
<template> 
   <v-content>
      <v-container fluid>
      

 <v-layout>
    <v-flex >
      <v-card>
        <v-container fluid grid-list-md>
          <v-layout row wrap>
            <v-flex
              xs12
              md6
              lg3
              v-for="n in 8"
              :key="n"
            >
             
                <single-card></single-card>
             
            </v-flex>
          </v-layout>
        </v-container>
        </v-card>
    </v-flex>
  </v-layout>


      </v-container>
    </v-content>
</template>

<script>
import SingleCard from './SingleCard.vue';
  export default {
    name:'ProductList',
    components: {
        SingleCard
    },
    data: () => ({
      loading: false,
      selection: 1,
      
    }),
    props: ['array']
  }
</script>
<style scoped>
.product-list{
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    padding-top: 5%;
}
</style>