<template>
  <v-container>
          
            <v-flex
              xs12
              md6
              lg3 
               v-for="(item,index) in items" :key="index"
            >

  <v-card >
    <v-img :src="require(`../../public/images/${item.image}`)"></v-img>


    <v-card-title>{{item.title}}</v-card-title>

    <v-card-text>
      

      <div class="my-4 text-subtitle-1">
        $ {{item.price}}
      </div>

      <div>{{item.description}}</div>
      <div><a href="">More details...</a></div>
    </v-card-text>

    <v-divider class="mx-4"></v-divider>
    <v-btn block>
    Add to cart
  </v-btn>
    
  </v-card>
 
    </v-flex>
         
        </v-container>
  
</template>

<script>
export default {
    name:'SingleCard',
    data() {
    return{ 
    loading: false,
    selection: 1, 
    items:[{
        id:'1',
        title: "Crunchy Bento box",
        description: "Aliquam erat volutpat. Ut fermentum orci eget dolor accumsan, sit amet dapibus lacus lobortis.",
        price: "750",
        stock:34,
        image:"sushi-1.jpeg"
    },

    {
        id:'2',
        title: "Nigiri Bento box",
        description: "Ut fermentum orci eget dolor accumsan, sit amet dapibus lacus lobortis.Aliquam erat volutpat.",
        price: "900",
        stock:15,
        image:"sushi-2.jpeg"
    },

    {
        id:'3',
        title: "Peruvian Bento box",
        description: "Nam dignissim dolor ut arcu malesuada, eget elementum felis eleifend. Suspendisse sollicitudin ex odio.",
        price: "840",
        stock:12,
        image:"sushi-3.jpeg"
    },

    {
        id:'4',
        title: "Tempura Bento box",
        description: "Suspendisse sollicitudin ex odio. Nam dignissim dolor ut arcu malesuada, eget elementum felis eleifend.",
        price: "670",
        stock:28,
        image:"sushi-4.jpeg"
    },

    {
        id:'5',
        title: "Salmon Bento box",
        description: "Sed auctor diam tellus, at eleifend leo imperdiet nec. Etiam elementum libero mauris.",
        price: "1100",
        stock:28,
        image:"sushi-5.jpeg"
    },

    {
        id:'6',
        title: "Meat Bento box",
        description: "Etiam elementum libero mauris. Sed auctor diam tellus, at eleifend leo imperdiet nec.",
        price: "1200",
        stock:23,
        image:"sushi-6.jpeg"
    },

    {
        id:'7',
        title: "Extras",
        description: "Soya sauce.",
        price: "350",
        stock:35,
        image:"salsa-soja.jpg"
    },

    {
        id:'8',
        title: "Extras",
        description: "Teriyaki sauce",
        price: "350",
        stock:15,
        image:"salsa-teriyaki.jpg"
    },

    {
        id:'9',
        title: "Extras",
        description: "Biterseweet sauce.",
        price: "350",
        stock:25,
        image:"salsa-agridulce.jpg"
    },

    {
        id:'10',
        title: "Extras",
        description: "Ginger.",
        price: "350",
        stock:14,
        image:"jengibre.jpg"
    },

    {
        id:'11',
        title: "Extras",
        description: "Wasabi.",
        price: "350",
        stock:46,
        image:"wasabi.jpg",
    }],
    }
    }
    }
</script>

