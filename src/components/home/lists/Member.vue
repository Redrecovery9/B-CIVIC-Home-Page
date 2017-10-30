<template>
  <div class='member'>
    <b-card class='card' title="Highlighted Members">
      <b-container class="card-body">
          <b-row>
            <b-col>
              <img class='image' fluid src="../../../assets/first_bank_logo.jpg" alt="Thumbnail" />
            </b-col>
            <b-col>
              <img class='image' fluid src="../../../assets/Davita.png" alt="Thumbnail" />
            </b-col>
            <b-col>
              <img class='image' fluid src="../../../assets/kaiser-permanente-logo.png" alt="Thumbnail" />
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

.image {
  max-width: 250px;
  height: auto;
}
</style>
