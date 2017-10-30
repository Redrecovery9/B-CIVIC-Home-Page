<template>
  <div>
    <Carousel class='carousel'/>
    <b-container class="bv-example-row">
      <b-row>
          <b-col class='twitter'><TwitterFeeds  :feeds='feeds'/></b-col>
          <b-col cols="11" class='cards'><Members/></b-col>
      </b-row>
      <b-row>
          <b-col class='twitter'><TwitterEvents/></b-col>
          <b-col cols="11" class='cards'><Events/></b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import Carousel from './home/Carousel'
import TwitterFeeds from './home/TwitterFeeds'
import TwitterEvents from './home/TwitterEvents'
import Members from './home/Members'
import Events from './home/Events'

export default {
  name: 'home',
  components: {
    Carousel,
    TwitterFeeds,
    TwitterEvents,
    Members,
    Events
  },
  data() {
    return {

    }
  },
}
</script>

<style>
.carousel {
  margin-top: 75px;
}

.twitter {
  margin-top: 10px;
  margin-left: -135px;
  margin-right: -20px
}

.cards {
  margin-top: 10px;
  margin-right: -115px;
}

</style>
