<template>
  <div class="twitterfeeds">
    <div class="title">
      <b-card title="B:CIVIC Feed">
        <TwitterFeed class='cards' v-for='feed in feeds' :feed="feed" key=''/>
      </b-card>
    </div>
  </div>
</template>

<script>
import TwitterFeed from './lists/TwitterFeed'

export default {
  name: 'TwitterFeeds',
  props: [],
  data() {
    return {
      feeds: [],
    }
  },
  components: {
    TwitterFeed
  },
  async mounted(){
    const data = await fetch(`https://bcivic-server.herokuapp.com/twitter/feed`)
    const response = await data.json()
    this.feeds = response
  },
}
</script>

<style scoped>
.twitterfeeds {
  margin-top: 15px;
}

.title {
  display: flex;
  justify-content: center;
}

h4.card-title {
  width: 85%;
  height: 40px;
  margin-top: -30px;
  background-color: white;
  font-weight: bold;
  color: #004286;
  position: absolute;
  z-index: 900;
}

.card-body {
  width: 330px;
  height: 343px;
  margin-top: 25px;
  overflow: scroll;
}

.cards {
  margin-top: 100px;
  width: 90%;
  margin-top: 15px;
}
</style>
