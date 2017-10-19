<template>
  <div class='event'>
    <b-card class='card' title="Upcoming Events">
      <span class='event-date'>Date: mm/dd/yyyy</span>
      <b-container class="card-body">
          <b-row>
              <b-col><img class='card-img' src="https://placekitten.com/1000/300" alt="Card image"></b-col>
              <b-col><p class="card-text">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
                enim ad minim veniam, quis nostrud exercitation ullamco laboris
                nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in
                reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
                pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
                culpa qui officia deserunt mollit anim id est laborum.
              </p></b-col>
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
}
</script>

<style scoped>
.event{
  margin-top: 33px;
}

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


</style>
