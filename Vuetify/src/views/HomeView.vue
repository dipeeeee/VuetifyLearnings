<script lang="ts">
  export default {
    data () {
      return {
        items: [
          {
            src: 'https://images2.alphacoders.com/127/thumb-1920-1274884.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
          },
          {
            src: 'https://images3.alphacoders.com/823/thumbbig-82317.webp',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
          },
        ],
      }
    },
  }
</script>

  <template>
  <v-carousel hide-delimiters>
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      cover
    ></v-carousel-item>
  </v-carousel>

   <div class="text-center text-h4 mt-5">My First Vuetify Website</div>

</template>
    
