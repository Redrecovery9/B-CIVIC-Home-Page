<template>
  <div class='event'>
    <b-card class='card' title="Upcoming Events">
      <span class='event-date'>Date: {{convention.date | moment("dddd, MMMM Do YYYY") }}</span>
      <b-container class="card-body">
          <b-row>
              <b-col><img class='card-img' src="../../../assets/BCIVIC-Summit-Logo.jpg" alt="Card image"></b-col>
              <b-col cols='7'>
                <h3>{{convention.name}}</h3>
                <p class="card-text">
                {{convention.description}}
              </p>
              <p class='keynotes'>Key Notes:
                <span class='keynote' v-for='people in convention.people' :people="people" key=''>{{people.name}}
                </span>
              </p>
              </b-col>
          </b-row>
      </b-container>
      <b-container class='card-link-con'>
        <a href="#" class="card-link">Event Info</a>
      </b-container>
    </b-card>
</div>
</template>

<script>
export default {
  props: ['convention']
}
</script>

<style scoped>

.card {
  font-weight: 600;
  color: #004286;
}

.event-date {
  font-weight: bold;
  color: #73DC44;
}

.card-text {
  font-weight: 400;
  color: black;
}

.card-link-con {
  display: flex;
  justify-content: flex-end;
}

.card-link {
  color: #004286;
}

.card-link:hover {
  color: #73DC44;
}

.card-img {
  max-width: 350px;
  height: auto;
}

.keynotes {
  display: inline-block;
  color: #73DC44
}

.keynote {
  color: #004286;
  margin-right: 20px;
}

</style>
