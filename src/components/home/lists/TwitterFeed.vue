<template>
  <div class='feed'>
    <b-card no-body class="text-center">
      @{{feed.user.screen_name}}  {{feed.created_at | moment(" MMM D YYYY") }}
      <br>
      {{feed.text}}
    </b-card>
  </div>
</template>

<script>
export default {
  props: ['feed']
}
</script>

<style scoped>
.text-center {
  font-size: .8em;
  margin-top: 3px;
}
</style>
