<template>
    <v-app>
 <div>
  <v-app-bar
      color="primary"
     
     
      
    >
      <nuxt-link to="../work1"><span class="material-icons" style="color:#ffffff;">keyboard_backspace</span></nuxt-link>

      <v-toolbar-title>Welcome</v-toolbar-title>

      <v-spacer></v-spacer>


      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-btn icon>
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
  </v-app-bar>
  <v-toolbar>
    <v-tabs
     
      background-color="primary "
      grow
     style="margin-top:-10px;"
    >
      <v-tab>
        
         SIGN UP
        
      </v-tab>

        

      <v-tab>
       
        SIGN IN
        
      </v-tab>
    </v-tabs>
  </v-toolbar>
    </div>

  <!-- Sizes your content based upon application components -->
  <v-main>
    <v-content>
      <nuxt/>
    </v-content>
  </v-main>

  

</v-app>
</template>