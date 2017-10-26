<template>
  <div class='member'>
    <b-card class='card' title="Highlighted Members">
      <b-container class="card-body">
          <b-row>
            <b-col>
              <b-img class='image' thumbnail fluid src="https://lorempixel.com/250/250/technics/4/" alt="Thumbnail" />
            </b-col>
            <b-col>
              <b-img class='image' thumbnail fluid src="https://lorempixel.com/250/250/technics/8/" alt="Thumbnail" />
            </b-col>
            <b-col>
              <b-img class='image' thumbnail fluid src="https://lorempixel.com/250/250/technics/4/" alt="Thumbnail" />
            </b-col>
          </b-row>
      </b-container>
    </b-card>
</div>
</template>

<script>
export default {
}
</script>

<style scoped>
.member{
  margin-top: 15px;
}

.card {
  font-weight: 600;
  color: #004286;
}
</style>
