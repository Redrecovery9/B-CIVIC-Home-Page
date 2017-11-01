<template>
  <div class='event'>
    <div class="title">
        <b-card no-body class="text-center">
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
.text-center {
  font-size: .8em;
  margin-top: 3px;
}
</style>
