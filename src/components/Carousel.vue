<template>

 <div>
    <Slider
      animation="fade"
      v-model="sliderValue"
      :duration="5000"
      :speed="1000"
    >
      <SliderItem
        v-for="slide in imageList"
        :key="slide.id"
      >

      <img :src="slide.url"/>

      </SliderItem>
    </Slider>
  </div>

</template>

<script>
import { Slider, SliderItem } from "vue-easy-slider";

export default {
  name: "carousel",
  components: {
    Slider,
    SliderItem
  },
  data() {
    return {
      imageList: [
          {
              url: require('@/assets/tab1.jpg'),
              id: 1
          },
          {
              url: require('@/assets/tab2.jpg'),
              id: 2
          },
          {
              url: require('@/assets/lap4.jpg'),
              id: 3
          }
      ],
    };
  },
}


</script>
<style  scoped>
img{
   
   width: 100% ;
   height: 100%;
}
</style>

