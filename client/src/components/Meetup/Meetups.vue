<template>
  <v-container>
    <v-layout row wrap>
      <v-flex xs12>
        <v-card class="info">
          <v-container fluid>
            <v-layout row>
              <v-flex xs5 sm4 md3>
                <v-card-media
                  src="https://upload.wikimedia.org/wikipedia/commons/4/47/New_york_times_square-terabass.jpg"
                  height="130px"
                  >
                </v-card-media>
              </v-flex>
              <v-flex xs7 sm8 md9>
                <v-card-title primary-title>
                  <div>
                    <h5 class="white--text mb0">My Meetup</h5>
                    <div>17th July 2018</div>
                  </div>
                </v-card-title>
                <v-card-action>
                  <div>
                  <v-btn flat>
                    <v-icon left light>arrow_forward</v-icon>
                    view Meetup
                  </v-btn>
                  </div>
                </v-card-action>
              </v-flex>
            </v-layout>
          </v-container>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>
