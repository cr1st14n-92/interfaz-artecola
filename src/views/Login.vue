<template>
    <v-container class="fill-height">
        <v-row
          align="center"
          justify="center"
        >
            <v-card width="500px" color="grey darken-4">

              <div style="text-align:center;padding-top:30px">
                 <img  width="250" src="https://cr1st14n-92.github.io/artecola/avatar/icons/marca.svg" />
              </div> 
                 <v-card-text>
                     <v-form>
                           <v-text-field
                    label="usuario"  
                    name="user"
                    prepend-inner-icon="mdi-account"
                    type="text"
                    solo
                  />

                  <v-text-field
                    id="password"
                  
                    label="clave"
                     color="primary"
                    name="password"
                    prepend-inner-icon="mdi-lock"
                    type="password"
                   
                    solo
                  />
                     </v-form>
                 </v-card-text>

                  <v-card-actions>
                <v-spacer />
                <v-btn   dark color="error" @click="autenticar">Autenticar</v-btn>
              </v-card-actions>
            </v-card>
        </v-row>
    </v-container>
</template>

<script>
export default {

  methods:{
    autenticar(){
      this.$router.push("/home");
    }
  }
    
}
</script>

<style>

</style>