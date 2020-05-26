<template>
  <div>
        <v-row
            key="ab4"
            class="mb-12"
            no-gutters
        >
        <v-col
            key="ab5"
            class="text-left"
        >
        <v-card>
            <v-chip
                class="ma-2"
                color="green"
                width="12"
                text-color="white"
            >
                {{label}}
            </v-chip>
        </v-card>
        </v-col>
        <v-col
            key="ab6"
            class="text-right"
        >
        <v-card>
            <v-chip
                class="ma-2"
                color="primary"
                text-color="white"
            >
                {{desc}}
            <v-icon right>mdi-cake-variant</v-icon>
            </v-chip>
        </v-card>
        </v-col>
        </v-row>
  </div>
</template>

<script>
export default {
    name: "FactsAboutMe",
    props: {
        label: String,
        desc: String
    }
}
</script>

<style>

</style>