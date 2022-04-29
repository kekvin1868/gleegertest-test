<template>
  <v-app>
    <v-app-bar color="white" height="84px" app>
      <div class="mx-4">
        <v-img
          v-bind:src="require('../src/assets/sparrow-logo.png')"
          class="pr-3 align-center"
          max-width="150px"
          max-height="64px"
        />
      </div>

      <v-div fluid class="mx-4" align-content="center">
        <v-div md="4" class="my-0 py-0">
          <div>
            <v-icon>mdi-bitcoin</v-icon>
            <v-text class="ml-1 font-weight-medium">Bitcoin</v-text>
          </div>
        </v-div>
        <v-div md="4" class="my-0 py-0">
          <div class="ml-1">
            <v-text class="font-weight-light text-h6">88,888</v-text>
            <v-text class="font-weight-light text-caption">.88</v-text>
          </div>
        </v-div>
      </v-div>

      <v-div fluid class="mx-4 ml-6" align-content="center">
        <v-div md="4" class="my-0 py-0">
          <div>
            <v-icon>mdi-ethereum</v-icon>
            <v-text class="ml-1 font-weight-medium">Ethereum</v-text>
          </div>
        </v-div>
        <v-div md="4" class="my-0 py-0">
          <div class="ml-1">
            <v-text class="font-weight-light text-h6">88,888</v-text>
            <v-text class="font-weight-light text-caption">.88</v-text>
          </div>
        </v-div>
      </v-div>

      <v-spacer></v-spacer>

      <v-row align="center" justify="space-between" no-gutters>
        <v-btn text rounded>
          <v-text class="font-weight-medium text-caption">ConvertNOW</v-text>
        </v-btn>

        <v-btn text rounded>
          <v-text class="font-weight-medium text-caption">Options</v-text>
        </v-btn>

        <v-btn text rounded>
          <v-text class="font-weight-medium text-caption">Funds</v-text>
        </v-btn>

        <v-btn text rounded>
          <v-text class="font-weight-medium text-caption">Support</v-text>
        </v-btn>

        <v-btn outlined rounded color="blue">
          <v-text class="font-weight-medium text-caption">Settlement Price</v-text>
        </v-btn>

        <v-btn icon>
          <v-icon dark>mdi-account</v-icon>
        </v-btn>
        
        <v-divider class="profile-divider" vertical />

        <v-btn icon>
          <v-icon dark>mdi-earth</v-icon>
        </v-btn>
      </v-row>
    </v-app-bar>

    <v-main>
      <HelloWorld/>
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>

<style>
.profile-divider{
  border-width: 1px !important;
}
</style>
