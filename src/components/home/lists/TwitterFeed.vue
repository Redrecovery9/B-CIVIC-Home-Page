<template>
  <div class='feed'>
    <b-card no-body class="text">
      @{{feed.user.screen_name}}
      {{feed.created_at | moment(" MMM D YYYY") }}
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
.text{
  font-size: .8em;
  margin-top: 3px;
}
</style>
