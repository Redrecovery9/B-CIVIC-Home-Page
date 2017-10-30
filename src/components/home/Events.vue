<template>
  <div class="events">
    <Event></Event>
  </div>
</template>

<script>
import Event from './lists/Event'

export default {
  name: 'Events',
  props: [],
  data() {
    return {
      convention,
    }
  },
  components: {
    Event,
  },
  // async mounted(){
  //   const data = await fetch(`https://bcivic-server.herokuapp.com/convention`)
  //   const response = await data.json()
  //   console.log(response);
  //   this.feeds = response
  // },
}
</script>

<style scoped>

</style>
