<template>
  <v-app-bar color="white" height="84px" app>
    <div class="mx-4" name="nav-logo">
      <v-img
        v-bind:src="require('../../src/assets/sparrow-logo.png')"
        class="pr-3 align-center"
        max-width="150px"
        max-height="64px"
      />
    </div>

    <v-row class="d-flex flex-rows mx-4" align-content="center">
      <v-col cols="6" class="my-0 py-0" name='bc-title-field'>
        <v-row align="center">
          <v-col cols="12" md="12" class="pb-0">
            <v-icon color="#FFCA28">mdi-bitcoin</v-icon>
            <span class="font-weight-medium">Bitcoin</span>
          </v-col>
          <v-col cols="12" md="12" class="pt-0 mb-1 px-0">
            <span class="ml-4 font-weight-light text-h6">88,888</span>
            <span class="font-weight-light text-caption">.88</span>
          </v-col>
        </v-row>
      </v-col>
      <v-col cols="6" class="my-0 py-0" name='bc-title-field'>
        <v-row align="center">
          <v-col cols="12" md="12" class="pb-0">
            <v-icon color="#C5CAE9">mdi-ethereum</v-icon>
            <span class="font-weight-medium">Ethereum</span>
          </v-col>
          <v-col cols="12" md="12" class="pt-0 mb-1 px-0">
            <span class="ml-4 font-weight-light text-h6">88,888</span>
            <span class="font-weight-light text-caption">.88</span>
          </v-col>
        </v-row>
      </v-col>
    </v-row>

    <div class="mx-4" align-content="center" name="ethereum-area">
      
    </div>

    <v-spacer></v-spacer>

    <div name="menu" class="d-flex justify-end align-center" no-gutters>
      <v-btn class="mx-2" text rounded>
        <span class="font-weight-medium text-caption">ConvertNOW</span>
      </v-btn>
      
      <v-btn class="mx-2" text rounded>
        <span class="font-weight-medium text-caption">Options</span>
      </v-btn>

      <v-btn class="mx-2" text rounded>
        <span class="font-weight-medium text-caption">Funds</span>
      </v-btn>

      <v-btn class="mx-2" text rounded>
        <span class="font-weight-medium text-caption">Support</span>
      </v-btn>

      <v-btn class="mx-2" outlined rounded color="blue">
        <span class="font-weight-medium text-caption">Settlement Price</span>
      </v-btn>

      <v-btn class="mx-2" icon>
        <v-icon dark>mdi-account</v-icon>
      </v-btn>

      <v-divider class="mx-2 profile-divider" vertical />

      <v-btn class="mx-2" icon>
        <v-icon dark>mdi-earth</v-icon>
      </v-btn>
    </div>
  </v-app-bar>
</template>

<script>
export default {
  name: 'AppNav',

  data: () => ({
    //
  }),
};
</script>
