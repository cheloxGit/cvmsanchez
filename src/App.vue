<template>
  <v-app id="inspire">
    <v-container 
      fill-height fluid
    >
      <v-row 
        align="center"
        justify="center"
      >
      <v-col>
            <v-card
              key="1"
              class="d-flex justify-center text-center"
              flat
              tile
            >
              <!-- vcard 1 : ListButtons -->
              <ListButtons />
              
              <!-- vcard 2 : Avatar -->
              <Avatar />

              <!-- vcard 3 : Contents -->
              <Contents />

            </v-card>
      </v-col>
      </v-row>
    </v-container>
    <v-footer app>
      <span>&copy; 2020</span>  
    </v-footer>
  </v-app>
</template>

<script>
import ListButtons from './components/ListButtons.vue';
import Avatar from './components/Avatar.vue';
import Contents from './components/Contents.vue';

  export default {
    name: 'LayoutsDemosBaselineFlipped',
    components: {
      ListButtons,
      Avatar,
      Contents
    },
    created () {
      this.$vuetify.theme.dark = true
    },
  }
</script>