<template>
  <div id="app">
    <Toolbar class='toolbar'/>
    <Carousel class='carousel'/>
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
    <Copyrightbar class='copyrightbar'/>



  </div>
</template>

<script>
import Toolbar from './components/Toolbar'
import Carousel from './components/Carousel'
import TwitterFeeds from './components/TwitterFeeds'
import TwitterEvents from './components/TwitterEvents'
import Members from './components/Members'
import Events from './components/Events'
import Copyrightbar from './components/Copyrightbar'

export default {
  name: 'app',
  components: {
    Toolbar,
    Carousel,
    TwitterFeeds,
    TwitterEvents,
    Members,
    Events,
    Copyrightbar
  }
}
</script>

<style>
#app {

}

.toolbar {
  background-color: white;
  width: 100%;
  position: fixed;
  top: 0;
  z-index: 1000;
}

.carousel {
  margin-top: 75px;
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
