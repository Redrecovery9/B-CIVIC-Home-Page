<template>
  <div class='carousel'>
    <div>
      <b-carousel id="carousel1"
                style="text-shadow: 1px 1px 2px #333;"
                controls
                indicators
                background="#ababab"
                :interval="10000"
                img-width="1024"
                img-height="480"
                v-model="slide"
                >
        <b-carousel-slide>
          <img slot="img" class="d-block img-fluid w-100" width="1024" height="480"
               src="../../assets/BCIVICPOCslide1.png" alt="image slot">
        </b-carousel-slide>
        <b-carousel-slide>
          <img slot="img" class="d-block img-fluid w-100" width="1024" height="480"
               src="../../assets/BCIVICPOCslide2.png" alt="image slot">
        </b-carousel-slide>
      </b-carousel>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {

    }
  },
}
</script>

<style scoped>

</style>
