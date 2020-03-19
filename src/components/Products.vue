<template>
 <div>
  <div>
    <b-row>
    <b-col class="mx-3" style="width: 18rem">
    <b-card-group class="mt-3 displaycard">
      <b-card
        
        
        header-bg-variant="secondary"
        header-text-variant="white"
        align="center"
      >
        <b-card> <img :src="products.imageLink" img-top style="height:150px">
        </b-card>
       <b-card-text>
        <h5 class="card-title">{{products.name}}</h5>
        <p>{{products.price}}</p>
        <p>{{products.specs}}</p>
        
       </b-card-text>
       <b-button href="#" variant="danger">Add to cat</b-button>
       
      </b-card>

    
    </b-card-group>
    </b-col>
    </b-row>
  </div>
  
  
</div>
</template>

<script>
export default {
  props: ['products']
}
</script>