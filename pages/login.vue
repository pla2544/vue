<template>
 <v-app>
   <v-card>
     <v-card-title>
       <h1>Login</h1>


     </v-card-title>
     <v-card-text>
       <v-form>
         <v-text-field label="Username" prepend-icon="account_circle" />
         <v-text-field type="password" label="Password" prepend-icon="lock" append-icon="visibility_off"/>
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
 </v-app>
</template>