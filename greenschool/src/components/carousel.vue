<template>
   <v-flex xs12 lg12 md12 style="width:500%;  margin: auto 0">
        <v-carousel cycle hide-delimiters style="width:100%; max-height:900px" class="white">
          <v-carousel-item v-for="(item,i) in items" :src="item.src" :key="i"></v-carousel-item>
        </v-carousel>
      </v-flex>
<!-- <v-card class=mt-2>
 <v-carousel
    cycle
    height="700"
    hide-delimiter-background
    show-arrows-on-hover
  >
    <v-carousel-item
     
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    >
     
    </v-carousel-item>
  </v-carousel>
</v-card> -->
<!-- <v-carousel>
    <v-carousel-item
  
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
     
        cycle
    height="400"
    hide-delimiter-background
    show-arrows-on-hover
   ></v-carousel-item>
  </v-carousel> -->
 
</template>

<script>
  export default {
    name: 'carousel',

    data: () => ({
     items: [
          {
            src: require('@/assets/1.jpg')
          },
          {
            src: require('@/assets/2.jpg'),
          },
          {
            src: require('@/assets/3.jpg'),
          },
          {
            src: require('@/assets/1.jpg'),
          },
        ],
    }),
  }
</script>
