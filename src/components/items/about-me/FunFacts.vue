<template>
<div>    
    <v-card-title>
        <v-chip
            class="ma-2"
            color="green lighten-1"
            text-color="white"
        >
        <v-avatar
            left
            class="green darken-1"
        >
        </v-avatar>
            {{funfacts_label}}
        </v-chip>
    </v-card-title>
    <v-card-text>
        <!-- Row 1 -->
        <v-row
            key="ff1"
            class="mb-6"
            no-gutters
        >
        <!-- Web Development -->
        <v-col
            key="ff2"
            class="text-left"
        >
            <v-card
                class="text-center"
                max-width="200"
            >
            <v-icon >mdi-album</v-icon>
            <v-card-text class="text--primary">
            <div>{{funfacts_one_number}}</div>
            <div>{{funfacts_one_desc1}}</div>
            <div>{{funfacts_one_desc2}}</div>
            </v-card-text>
            </v-card>
        </v-col>
        <v-divider
            class="mx-4"
            vertical
        ></v-divider>
        <!-- Mobile Hybrid Development -->
        <v-col
            key="ff3"
            class="text-left"
        >
            <v-card
                class="text-center"
                max-width="200"
            >
            <v-icon >mdi-album</v-icon>
            <v-card-text class="text--primary">
            <div>{{funfacts_two_number}}</div>
            <div>{{funfacts_two_desc1}}</div>
            <div>{{funfacts_two_desc2}}</div>
            </v-card-text>
            </v-card>
        </v-col>
        <v-divider
            class="mx-4"
            vertical
        ></v-divider>
        <v-col
            key="ff4"
            class="text-left"
        >
            <v-card
                class="text-center"
                max-width="200"
            >
            <v-icon >mdi-album</v-icon>
            <v-card-text class="text--primary">
            <div>{{funfacts_three_number}}</div>
            <div>{{funfacts_three_desc1}}</div>
            <div>{{funfacts_three_desc2}}</div>
            </v-card-text>
            </v-card>
        </v-col>
        <v-divider
            class="mx-4"
            vertical
        ></v-divider>
        <v-col
            key="ff5"
            class="text-left"
        >
            <v-card
                class="text-center"
                max-width="200"
            >
            <v-icon >mdi-album</v-icon>
            <v-card-text class="text--primary">
            <div>{{funfacts_four_number}}</div>
            <div>{{funfacts_four_desc1}}</div>
            <div>{{funfacts_four_desc2}}</div>
            </v-card-text>
            </v-card>
        </v-col>
        </v-row>
    </v-card-text>
</div>
</template>

<script>
export default {
  name: "FunFacts",
   data: () => ({
        funfacts_label: 'Fun Facts',
        funfacts_one_number:'80',
        funfacts_one_desc1: 'Albumes',
        funfacts_one_desc2: 'Listened',
        funfacts_two_number:'80',
        funfacts_two_desc1: 'Albumes',
        funfacts_two_desc2: 'Listened',
        funfacts_three_number:'80',
        funfacts_three_desc1: 'Albumes',
        funfacts_three_desc2: 'Listened',
        funfacts_four_number:'80',
        funfacts_four_desc1: 'Albumes',
        funfacts_four_desc2: 'Listened',
    })
}
</script>

<style>

</style>