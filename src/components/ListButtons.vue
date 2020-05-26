<template>
    <v-card
      max-width="250"
      tile
    >
      <v-list rounded>
        <v-list-item-group color="primary">
          <v-list-item
            v-for="(item, i) in items"
            :key="i"
            v-on:click="goTo(item.key)"
          >
            <v-list-item-icon>
              <v-icon v-text="item.icon"></v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title v-text="item.text"></v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-card>
</template>

<script>
export default {
  name: "ListButtons",
  data: () => ({
      items: [
        { text: 'About Me', icon: 'mdi-account', key: 'aboutme'},
        { text: 'Resume', icon: 'mdi-clock', key: 'resume'},
        { text: 'Works', icon: 'mdi-flag', key: 'works'},
      ],
  }),
  methods: {
    goTo (key) {
        console.log('ListButtons [key]: '+ key)
        this.$root.$emit('changeAM',key);
    }
  }
};
</script>
