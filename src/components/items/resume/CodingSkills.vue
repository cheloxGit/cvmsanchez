<template>
  <div> 
        
        <v-row
            key="ms13"
            class="mb-6"
            no-gutters
        >
        <v-col
            key="ms14"
            class="text-center"
        >
        <v-progress-circular
            rotate="0"
            size="64"
            value="65"
            width="4"
            color="green"
        >{{number_one}}</v-progress-circular>
        </v-col>
        <v-divider vertical></v-divider>
        <v-col
            key="ms15"
            class="text-center"
        >
        <v-progress-circular
            rotate="0"
            size="64"
            value="65"
            width="4"
            color="green"
        >{{number_two}}</v-progress-circular>
        </v-col>
        </v-row>
        <v-row
            key="ms16"
            class="mb-6"
            no-gutters
        >
        <v-col
            key="ms17"
            class="text-center"
        >{{label_one}}</v-col>
        <v-col
            key="ms18"
            class="text-center"
        >{{label_two}}</v-col>
        </v-row>
       
  </div>
</template>

<script>
export default {
    name: "CodingSkills",
    props: {
        number_one: String,
        label_one: String,
        number_two: String,
        label_two: String,
    }
}
</script>

<style>

</style>