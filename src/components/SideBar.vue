<template>
  <v-navigation-drawer 
    width="312px"
    permanent
    color="indigo lighten-5"
  >
    <v-list dense nav>
      <v-list-item-group
        v-model="value"
        active-class="ch-currentbg"
      >
        <v-list-item 
          v-for="(item, i) in items"
          :key="i"
          class="py-1 mx-6 my-5"
        >
          <v-list-item-title 
            class="font-weight-light text-subtitle-1"
          >
            {{ item.title }}
          </v-list-item-title>
          
          <v-list-item-action v-if="item.title === 'Identity Verification'">
            <v-icon color="#69F0AE">
              {{ item.icon }}
            </v-icon>
          </v-list-item-action>

          <v-list-item-action v-else-if="item.title === 'Security'">
            <v-icon color="#FF5252">
              {{ item.icon }}
            </v-icon>
          </v-list-item-action>

          <v-list-item-action v-else>
            <v-icon>
              {{ item.icon }}
            </v-icon>
          </v-list-item-action>
        </v-list-item>
      </v-list-item-group>
    </v-list>
  </v-navigation-drawer>
</template>

<script>
  export default {
    name: 'SideBar',

    data: () => ({
      items: [
        { title: 'Accounts', icon: ''},
        { title: 'Activities', icon: ''},
        { title: 'API Management', icon: ''},
        { title: 'Address Management', icon: ''},
        { title: 'Identity Verification', icon: 'mdi-check-circle'},
        { title: 'Preferences', icon: ''},
        { title: 'Security', icon: 'mdi-alert-circle'},
      ],
      value: 0,
    }),
  }
</script>

<style>
.ch-currentbg {
  background-color: #2962FF;
  color: white !important;
}
</style>
