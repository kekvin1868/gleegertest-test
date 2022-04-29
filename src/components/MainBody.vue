<template>
  <v-container fluid>
    <v-row class="mx-3 my-3">
      <v-col class="pl-8 pt-6" cols="5">
        <p 
          style="color: #2962FF"
          class="text-h2 font-weight-normal"
        >
          Welcome.
        </p>
      </v-col>
      <v-col class="pt-6" cols="7">
        <v-card class="user-status-info" rounded color="#2962FF">

          <v-row class="d-flex ml-1">
            <v-col cols="7" class="pb-0">
              <v-card-title class="py-0">
                <span class="text-subtitle-1 white--text ">
                  Email
                </span>
              </v-card-title>
            </v-col>
            <v-col cols="5" class="pb-0">
              <v-card-title class="py-0">
                <span class="text-subtitle-1 white--text">
                  Country
                </span>
              </v-card-title>
            </v-col>
          </v-row>

          <v-row class="d-flex ml-1">
            <v-col cols="7" class="py-0">
              <v-card-title class="py-0">
                <span class="font-weight-black white--text">
                  Test@sparrowexchange.com
                </span>
              </v-card-title>
            </v-col>
            <v-col cols="5" class="py-0">
              <v-card-title class="py-0">
                <span class="font-weight-black white--text">
                  IDN
                </span>
              </v-card-title>
            </v-col>
          </v-row>

          <v-row class="d-flex ml-1">
            <v-col cols="7" class="pb-0">
              <v-card-title class="pb-0">
                <span class="text-subtitle-1 white--text ">
                  User ID
                </span>
              </v-card-title>
            </v-col>
            <v-col cols="5" class="pb-0">
              <v-card-title class="pb-0">
                <span class="text-subtitle-1 white--text">
                  Joined Since
                </span>
              </v-card-title>
            </v-col>
          </v-row>

          <v-row class="d-flex ml-1">
            <v-col cols="7" class="py-0">
              <v-card-title class="py-0">
                <span class="font-weight-black white--text">
                  00ddd4c4-b0b3-4df3-a694
                </span>
              </v-card-title>
            </v-col>
            <v-col cols="5" class="py-0">
              <v-card-title class="py-0">
                <span class="font-weight-black white--text">
                  12 Feb 21
                </span>
              </v-card-title>
            </v-col>
          </v-row>

          <v-row class="d-flex ml-1">
            <v-col cols="7" class="pb-0">
              <v-card-title class="pb-0">
                <span class="text-subtitle-1 white--text ">
                  Account Status
                </span>
              </v-card-title>
            </v-col>
            <v-col cols="5" class="pb-0">
              <v-card-title class="pb-0">
                <span class="text-subtitle-1 white--text">
                  2FA Status
                </span>
              </v-card-title>
            </v-col>
          </v-row>

          <v-row class="d-flex ml-1">
            <v-col cols="7" class="py-0">
              <v-card-title class="pt-0">
                <v-icon color="green" class="mr-2">mdi-checkbox-blank-circle</v-icon>
                <span class="font-weight-black white--text">
                  Verified
                </span>
              </v-card-title>
            </v-col>
            <v-col cols="5" class="py-0">
              <v-card-title class="pt-0">
                <v-icon color="red" class="mr-2">mdi-checkbox-blank-circle</v-icon>
                <span class="font-weight-black white--text">
                  Disabled
                </span>
              </v-card-title>
            </v-col>
          </v-row>

        </v-card>
      </v-col>
    </v-row>

    <v-container>
      <v-row class="mx-3">
        <v-col class="pl-8" cols="5">
          <v-list dense>
            <v-list-item class="activity-list">
              <v-list-item-title>
                <span class="text-h5">
                  Last Login
                </span>
              </v-list-item-title>
              
              <v-btn text>
                <span 
                  style="color: #2962FF"
                  class="text-caption text-weight-light"
                >
                  See all activities
                </span>
              </v-btn>
            </v-list-item>

            <v-list-item class="activity-list">
              <v-divider></v-divider>
            </v-list-item>

            <v-list-item class="activity-list">
              <v-list-item-subtitle>
                <span>30 Jan 21, 16:28, Chrome Mac OS X</span>
              </v-list-item-subtitle>
            </v-list-item>
          </v-list>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
export default {
  name: 'MainBody',

  data: () => ({
    //
  }),
};
</script>
