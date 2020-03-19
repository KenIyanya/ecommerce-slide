<template>
  <b-container fluid style="padding: 0">
  <!-- Content here -->
    <div id="app">
   
       <Header/>
       
        <b-row class="mt-3">
          <b-col cols="2" offset="1">
            <Category v-for="cat in categories" :categories="cat" :key="cat.id" /> 
          </b-col> 

          <b-col cols="7" offset="1">
           <Carousel/>
          </b-col>
        </b-row>
           
           <b-row align-h="center">
               <Products v-for="product in products" :products="product" :key="product.id"/>
           </b-row>
    
    </div>
    <Footer/>
    
  </b-container>
  
 
</template>

<script>

import Header from '@/components/Header.vue'
import Category from '@/components/Category.vue'
import Products from '@/components/Products.vue'
import Carousel from '@/components/Carousel.vue'
import Footer from './components/Footer'


export default {
  name: 'App',
  components: {
    Header,
    Category,
    Products,
    Carousel,
    Footer
    
  },
  data(){
    return{
      categories: [
        {
          
        id: 1, 
        name: "Computing"
      },{
        id: 2, 
        name: "Tablet/Phones"
      },
      {
        id: 3, 
        name: "Fashion"
      },
      {
        id: 4, 
        name: "Accessories"
      },
      

      ],
      products:[{
       imageLink: require('@/assets/lap1.jpg'),
        name: "hp 15",
        price: "$ 200",
        specs: "1TB HDD, 16GB RAM",
        categoryId: 1

      },
      {
       id: 2,
          imageLink : require('@/assets/lap1.jpg'),
          name : "hp 15",
          price: "$ 150",
          specs : "1TB HDD, 4GBRAM",
           
      },
       {
        id: 3,
          imageLink : require('@/assets/lap3.jpg'),
          name : "hp 15",
          price: "$ 180",
           specs : "1TB HDD, 16GBRAM",
      },
       {
       id: 4,
          imageLink : require('@/assets/lap3.jpg'),
          name : "hp 15",
          price: "$ 170",
          specs : "500GB HDD, 8GBRAM",
      },
       {
        id: 5,
          imageLink : require('@/assets/lap3.jpg'),
          name : "hp 15",
          price: "$ 150",
          specs : "500gb HDD, 4GB RAM",
      },
      {
        id: 6,
          imageLink : require('@/assets/pb1.jpg'),
          name : "Phone",
          price: "$ 150",
          specs : "32gb HDD, 4GB RAM",
      },
      {
        id: 7,
          imageLink : require('@/assets/tab1.jpg'),
          name : "Phone",
          price: "$ 150",
          specs : "32gb HDD, 4GBRAM",
      },
      {
        id: 8,
          imageLink : require('@/assets/tab2.jpg'),
          name : "hp 15",
          price: "$ 150",
          specs : "32gb HDD, 4GBRAM",
      },
      {
        id: 9,
          imageLink : require('./assets/tab2.jpg'),
          name : "iphone",
          price: "$ 550",
          specs : "64gb HDD, 6GB RAM",
      },
      

      
      ]
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap');
</style>
