<template>
  <div class="events">
    <Event v-for='convention in conventions' :convention="convention" key=''></Event>
  </div>
</template>

<script>
import Event from './lists/Event'

export default {
  name: 'Events',
  props: [],
  data() {
    return {
      conventions: [],
    }
  },
  components: {
    Event,
  },
  async mounted(){
    const data = await fetch(`https://bcivic-server.herokuapp.com/convention`)
    const response = await data.json()
    this.conventions = response
  },
}
</script>

<style scoped>

</style>
