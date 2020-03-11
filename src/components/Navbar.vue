<template>
    <nav>
        <v-toolbar flat color="error">

            <v-app-bar-nav-icon  @click="drawer = !drawer"></v-app-bar-nav-icon>
        </v-toolbar>
        
          <v-navigation-drawer app 
          v-model="drawer"        
          >

                    <v-list dense>
                      <v-subheader>REPORTS</v-subheader>
                    </v-list>
          </v-navigation-drawer>
        
    </nav>
</template>


<script>
export default {
  data: () => ({
    drawer:false
  }),
}
</script>