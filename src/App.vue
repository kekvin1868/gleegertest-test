<template>
  <v-app>
    <v-app-bar color="white" height="84px" app>
      <div class="mx-4" name="nav-logo">
        <v-img
          v-bind:src="require('../src/assets/sparrow-logo.png')"
          class="pr-3 align-center"
          max-width="150px"
          max-height="64px"
        />
      </div>

      <div class="mx-4" align-content="center" name="bitcoin-area">
        <div md="4" class="my-0 py-0" name='bc-title-field'>
          <v-icon color="#FFCA28">mdi-bitcoin</v-icon>
          <span class="ml-1 font-weight-medium">Bitcoin</span>
        </div>
        <div md="4" class="my-0 py-0" name="bc-currency-field">
          <span class="font-weight-light text-h6">88,888</span>
          <span class="font-weight-light text-caption">.88</span>
        </div>
      </div>

      <div class="mx-4" align-content="center" name="ethereum-area">
        <div md="4" class="my-0 py-0" name="eth-title-field">
          <v-icon color="#C5CAE9">mdi-ethereum</v-icon>
          <span class="ml-1 font-weight-medium">Ethereum</span>
        </div>
        <div md="4" class="my-0 py-0" name="eth-currency-field">
          <span class="font-weight-light text-h6">88,888</span>
          <span class="font-weight-light text-caption">.88</span>
        </div>
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

    <v-main>
      <div class="main-height d-flex">
        <div name="sidebar">
          <SideBar />
        </div>
        <div name="mainbody">
          <MainBody />
        </div>
      </div>
    </v-main>
  </v-app>
</template>

<script>
import SideBar from './components/SideBar';
import MainBody from './components/MainBody';

export default {
  name: 'App',

  components: {
    SideBar,
    MainBody,
  },

  data: () => ({
    //
  }),
};
</script>

<style scoped>
.profile-divider {
  border-width: 1px !important;
}

.main-height {
  height: 100%;
}
</style>
calc(100vh - 97px)
