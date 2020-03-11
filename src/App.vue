<template>
  <v-app>
<v-content>
    <Navbar  v-if= "['Login'].indexOf($route.name) == -1"></Navbar>
   <router-view></router-view>

   </v-content>
  </v-app>
</template>

<script>
//import HelloWorld from './components/HelloWorld';
import Navbar from './components/Navbar'

export default {
  name: 'App',
  components: {
    Navbar
  },
  data: () => ({
    //
  }),
};
</script>
