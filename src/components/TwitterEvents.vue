<template>
  <div class="twitterevents">
      <div class="title">
        <b-card title="B:CIVIC Events">
          <TwitterEvent class='cards' v-for='feed in feeds' :feed="feed" key=''/>
        </b-card>
      </div>
  </div>
</template>

<script>
import TwitterEvent from './lists/TwitterEvent'

export default {
  name: 'TwitterEvents',
  components: {
    TwitterEvent
  }
}
</script>

<style scoped>

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
  color: #73DC44;
  position: absolute;
  z-index: 900;
}

.card-body {
  width: 330px;
  height: 334px;
  margin-top: 25px;
  overflow: scroll;
}

.cards {
  margin-top: 100px;
  width: 90%;
  margin-top: 15px;
}
</style>
