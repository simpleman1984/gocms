<template>
  <b-carousel id="carousel1"
              style="text-shadow: 1px 1px 2px #333;"
              controls
              indicators
              background="#ababab"
              :interval="4000"
              img-width="1024"
              img-height="480"
              v-model="slide"
              @sliding-start="onSlideStart"
              @sliding-end="onSlideEnd"
  >

    <!-- Text slides with image -->
    <b-carousel-slide caption="First slide"
                      text="Nulla vitae elit libero, a pharetra augue mollis interdum."
                      img-src="https://placekitten.com/1024/480"
    ></b-carousel-slide>

  </b-carousel>
</template>
<script>
  export default {
    data () {
      return {
        slide: 0,
        sliding: null
      }
    },
    methods: {
      onSlideStart (slide) {
        this.sliding = true
      },
      onSlideEnd (slide) {
        this.sliding = false
      }
    }
  }
</script>

