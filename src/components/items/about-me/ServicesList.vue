<template>
  <div>
        <v-divider class="ma-8" inset></v-divider>
        <v-row
            key="ms1"
            class="mb-6"
            no-gutters
        >
       
        <v-col
            key="ms2"
            class="text-left"
        >
           
            <v-card
                class="mx-auto"
                max-width="200"
            >
           
            <v-img
                class="white--text align-end"
                height="100px"
                :src="src_bg_one"
            >
                <v-card-title>{{title_one}}</v-card-title>
            </v-img>
            <v-card-subtitle class="pb-0">{{subtitle_one}}</v-card-subtitle>
            <v-card-text class="text--primary">
                <div>{{desc_one}}</div>
            </v-card-text>
            </v-card>       
        </v-col>
        <v-divider
            class="mx-4"
            vertical
        ></v-divider>
        <v-col
            key="ms3"
            class="text-left"
        >
            <v-card
                class="mx-auto"
                max-width="200"
            >
            <v-img
                class="white--text align-end"
                height="100px"
                :src="src_bg_two"
            >
                <v-card-title>{{title_two}}</v-card-title>
            </v-img>
            <v-card-subtitle class="pb-0">{{subtitle_two}}</v-card-subtitle>
            <v-card-text class="text--primary">
                <div>{{desc_two}}</div>
            </v-card-text>
            </v-card> 
        </v-col>
        </v-row>
      
  </div>
</template>

<script>

export default {
    name: "ServicesList",
    props: {
        title_one: String,
        src_bg_one: String,
        subtitle_one: String,
        desc_one:String,
        title_two: String,
        src_bg_two: String,
        subtitle_two: String,
        desc_two:String
    },
}
</script>

<style>

</style>