<template>
  <div class='event'>
    <div class="title">
        <b-card class="text-center">
          {{ hashtag.text }}
        </b-card>
      </b-card>
    </div>
  </div>
</template>

<script>
export default {
  props: ['hashtag']
}
</script>

<style scoped>
.title {
  display: flex;
  justify-content: center;
}

h4 {
  font-weight: bold;
  color: #73DC44;
}
</style>
