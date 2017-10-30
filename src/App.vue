<template>
  <div id="app">
    <Toolbar class='toolbar'/>
    <router-view/>
    <Copyrightbar class='copyrightbar'/>
  </div>
</template>

<script>
import Toolbar from './components/Toolbar'
import Copyrightbar from './components/Copyrightbar'

export default {
  name: 'app',
  components: {
    Toolbar,
    Copyrightbar
  },
  data() {
    return {

    }
  },
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

</style>
