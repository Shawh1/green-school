<template>
<v-carousel>
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
    ></v-carousel-item>
  </v-carousel>

</template>

<script>
  export default {
    name: 'carousel',

    data: () => ({
     items: [
          {
            src: 'https://github.com/Shawh1/green-school/blob/master/greenschool/src/assets/1.jpg'
          },
          {
            src: 'https://github.com/Shawh1/green-school/blob/master/greenschool/src/assets/1.jpg',
          },
          {
            src: 'https://github.com/Shawh1/green-school/blob/master/greenschool/src/assets/1.jpg',
          },
          {
            src: 'https://github.com/Shawh1/green-school/blob/master/greenschool/src/assets/1.jpg',
          },
        ],
    }),
  }
</script>
