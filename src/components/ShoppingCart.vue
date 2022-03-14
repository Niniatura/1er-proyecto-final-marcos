<template>
  <v-navigation-drawer
      app
      color="grey lighten-3"
      right
      width="360"
    >
    <v-toolbar class="pl-0 mt-5" flat color="grey lighten-3">
                <h3>My Order</h3>
                <v-spacer></v-spacer>
                <h6 class="green--text">Edit</h6>
    </v-toolbar>
     <v-app-bar flat color="rgba(0,0,0,0)" class="mt-n5">
              <v-btn fab x-small color="green lighten-4" elevation="0">
                <v-icon color="green">fas fa-clock</v-icon>
              </v-btn>
              <h5 class="ml-2 grey--text text--darken-2"> 14.30 AM</h5>
               
            </v-app-bar>
             <v-app-bar flat color="rgba(0,0,0,0)" class="mt-n5">
              <v-btn fab x-small color="green lighten-4" elevation="0">
                <v-icon color="green">fas fa-map-marker-alt</v-icon>
              </v-btn>
              <h5 class="ml-2 grey--text text--darken-2"> Ayacucho 8930, CABA</h5>
               
            </v-app-bar>
            <v-divider></v-divider>
             
                 <v-container >
                     <v-row>
                         
                        <v-col cols="12" sm="3">
                            <v-img src="../../public/images/sushi-4.jpeg"  max-height="90" max-width="90" contain class="mt-1 mr-1"></v-img>
                        </v-col>
                         <v-col cols="12" sm="3">
                            <h6 class="ml-n6 grey--text text--darken-2">Tempura Bento box</h6>
                         </v-col>
                         <v-col cols="12" sm="6">
                            <v-btn class="btn" x-small>+</v-btn>
                         <v-divider vertical inset class="mr-1"></v-divider>
                         1
                         <v-divider vertical inset class="mr-1"></v-divider>
                         <v-btn class="btn" x-small>-</v-btn>
                          
                        <v-divider vertical inset class="mr-1"></v-divider>
                         <v-btn class="btn" x-small>x</v-btn>
                        <v-divider vertical inset class="mr-1"></v-divider>
                         <v-toolbar class="pl-0" flat color="grey lighten-3">
                            <v-spacer></v-spacer>
                                <strong class="ml-1 mr-1 right">$670</strong>
                         </v-toolbar>     
                         </v-col>
                        
                     </v-row>
                       </v-container>
             <v-divider></v-divider>         
           <v-toolbar class="pl-0" flat color="grey lighten-3">
                <h3>Total</h3>
                <v-spacer></v-spacer>
                <h3>$670</h3>
            </v-toolbar>
          <div class="text-center">
                    <v-btn block>
                    Checkout
                    </v-btn>
          </div>         
    </v-navigation-drawer>
</template>

<script>
  export default {
    name:'ShoppingCart'
  }
</script>