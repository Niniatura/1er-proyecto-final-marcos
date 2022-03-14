<template>
  <v-container>
          
            <v-flex
              xs12
              md12
              lg12
            >

  <v-card >
   <v-row>
    <v-col class="col-6 col-md-4" >
    <v-img src="../../public/images/sushi-4.jpeg" max-height="200" max-width="200"></v-img>
    </v-col>
    <v-col class="col-12 col-sm-6 col-md-8">
    <v-card-title>Tempura Bento box</v-card-title>
    <div    >Sollicitudin ex odio. Nam dignissim dolor ut arcu malesuada, eget elementum felis eleifend.Suspendisse sollicitudin ex odio. Nam dignissim dolor ut arcu malesuada, eget elementum felis eleifend.</div>
    </v-col>
   </v-row>

    <v-card-text>
      

     <div class="mr-5 my-4 text-subtitle-1 text-right">
        <strong>$670</strong>
      </div>
    </v-card-text>
    <v-toolbar class="pl-0" flat color="grey lighten-3">
    <v-btn elevation="2">Back to list</v-btn>
     <v-spacer></v-spacer>
      <v-btn elevation="2">Add to cart</v-btn>
    </v-toolbar>
   
  </v-card>
 
    </v-flex>
         
        </v-container>
  
</template>

<script>
  export default {
    name:'ProductDetail'
  }
</script>