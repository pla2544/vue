<template>
 <v-app>
     <center>
         <br>
   <v-card width="400" color="#D2691E">
       
     <v-card-title>
       <h1>Login</h1>
     </v-card-title>

     <v-card-text>
       <v-form>
         <v-text-field label="Username" prepend-icon="account_circle" />
         <v-text-field 
            :type="showPassword ? 'text' : 'password'" 
            label="Password"
            prepend-icon="mdi-lock"
            :append-icon="showPassword ? 'mdi-eye' : 'mdi-eye-off'"
            @click:append="showPassword = !showPassword"
          />
       </v-form>
     </v-card-text>
     <v-card-actions>
         <nuxt-link to="/#/">
    <v-btn class="ma-2" tile color="green darken-4" dark>REGISTER</v-btn>
    </nuxt-link>
         <v-spacer></v-spacer>
         <v-btn color="info">login </v-btn>
     </v-card-actions>
   </v-card>
   </center>
 </v-app>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      showPassword: false
    }
  }
}
</script>