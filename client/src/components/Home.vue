<template>
  <v-container>
    <v-layout row wrap>
      <v-flex xs12 sm6 class="text-xs-center text-sm-right">
        <v-btn large to="/meetups" class="blue lighten-2" dark>Explore Meetups</v-btn>
      </v-flex>
      <v-flex xs12 sm6 class="text-xs-center text-sm-left">
        <v-btn large to="/meetup/new" class="blue lighten-2" dark>Organize Meetup</v-btn>
      </v-flex>
    </v-layout>
    <v-layout row wrap class="mt-2">
      <v-flex xs12>
        <v-carousel light>
          <v-carousel-item
            v-for="meetup in meetups"
            :src="meetup.imageUrl"
            :key="meetup.id"
            contain>
            <!-- <v-card-media
              :src="meetup.imageUrl"
              height="500px"
              > -->
            <div class="judul">
              <p>{{meetup.title}}</p>
            </div>
            <!-- </v-card-media> -->
          </v-carousel-item>
        </v-carousel>
      </v-flex>
    </v-layout>
    <v-layout row wrap class="mt-2">
      <v-flex xs12 class="text-xs-center">
        <p>Join our awesome meetups!</p>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data () {
    return {
      meetups: [
        {
          imageUrl: 'https://upload.wikimedia.org/wikipedia/commons/4/47/New_york_times_square-terabass.jpg',
          id: 'afajr',
          title: 'Meetup in New York'
        },
        {
          imageUrl: 'https://static.pexels.com/photos/338515/pexels-photo-338515.jpeg',
          id: 'afajro',
          title: 'Meetup in Paris'
        },
        {
          imageUrl: 'https://c1.staticflickr.com/2/1423/1202039057_986bb35857_b.jpg',
          id: 'afajrddo',
          title: 'Meetup in Indonesia'
        }
      ]
    }
  }
}
</script>

<style scoped>
.judul {
  /* position: absolute; */
  /* position: bottom; */
  /* offset-block-start: 20%; */
  /* position: fixed; */
  bottom: 50px;
  /* margin-top: 90%; */
  /* margin-left: 35%; */
  /* margin-right: 35%; */
  background-color: rgba(0, 0, 0, 0.5);
  color: white;
  font-size: 2em;
  padding: 20px;
}
/* .carousel {
  height:500px;
  width:100%;
} */
</style>
