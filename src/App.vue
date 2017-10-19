<template>
  <div id="app">
    <Toolbar/>
    <Carousel/>
    <b-container class="bv-example-row">
      <b-row>
          <b-col class='twitter'><TwitterFeeds/></b-col>
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
import Toolbar from './components/Toolbar'
import Carousel from './components/Carousel'
import TwitterFeeds from './components/TwitterFeeds'
import TwitterEvents from './components/TwitterEvents'
import Members from './components/Members'
import Events from './components/Events'
import Footer from './components/Footer'

export default {
  name: 'app',
  components: {
    Toolbar,
    Carousel,
    TwitterFeeds,
    TwitterEvents,
    Members,
    Events,
    Footer
  }
}
</script>

<style>
#app {

}

.twitter {
  margin-top: 10px;
  margin-left: -150px;
  margin-right: -20px
}

.cards {
  margin-top: 10px;
  margin-right: -150px;
}
</style>
