<template>
  <v-app>
    <v-main>
      <HelloWorld/>
      <AllUsers/>
    </v-main>
  </v-app>
</template>

<script>
import AllUsers from './modules/excel/pages/AllUsers.vue'
export default {
  name: 'App',
  components: {
    AllUsers
  },

  data: () => ({
    //
  }),
}
</script>
