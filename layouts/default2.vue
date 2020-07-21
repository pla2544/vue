<template>
<v-app>
     <v-system-bar
          color="#3F51B5"
          :height="height"
          :lights-out="lightsOut"
          :window="window"
        >
          <v-icon>mdi-gmail</v-icon>
          <span>10 unread emails</span>
          <v-spacer></v-spacer>
          <v-icon>mdi-wifi-strength-4</v-icon>
          <v-icon>mdi-signal-cellular-outline</v-icon>
          <v-icon>mdi-battery</v-icon>
          <span>12:30</span>
        </v-system-bar>
  <div>
    <v-toolbar>
    <v-tabs
      dark
      background-color="#5C6BC0"
      grow
    >
      <v-tab>
        
         Home
       
      </v-tab>

      <v-tab>
       
         Profile
       
      </v-tab>

      <v-tab>
        
         Login
       
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

    <v-footer
    color="#5C6BC0"
    padless
  >
    <v-row
      justify="center"
      no-gutters
    >
      <v-btn
        v-for="link in links"
        :key="link"
        color="white"
        text
        rounded
        class="my-2"
      >
        {{ link }}
      </v-btn>
      
    </v-row>
  </v-footer>
</v-app>

</template>
<script>
  export default {
    data: () => ({
      links: [
        'Home',
        'About Us',
        'Team',
        'Services',
        'Blog',
        'Contact Us',
      ],
    }),
  }
</script>