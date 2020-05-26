<template>
  <div>
    <v-card-title>
        <v-chip
            class="ma-2"
            color="green lighten-1"
            text-color="white"
        ><v-avatar
            left
            class="green darken-1"
        ></v-avatar>{{testimonials_label}}
        </v-chip>
    </v-card-title>
    <v-card-text>
        <!-- Row 1 -->
        <v-carousel
            cycle
            height="400"
            hide-delimiter-background
            show-arrows-on-hover
        >
            <v-carousel-item
                v-for="(slide, i) in slides"
                :key="i"
            >
            <v-sheet
                :color="color"
                height="50%"
            >
                <v-row
                    class="fill-height display-3"
                    align="center"
                    justify="center"
                >
                    <div>{{ slide.testimonial }}</div>
                </v-row>
                <v-row
                    align="center"
                    justify="center"
                >
                    <div class="display-1">{{ slide.name }}</div>
                </v-row>
            </v-sheet>
            </v-carousel-item>
        </v-carousel>
    </v-card-text>
  </div>
</template>

<script>
export default {
 name: "Testimonials",
 data: () => ({
    testimonials_label: 'Testimonials',
    color: 'gray',
    slides: [
        {name: 'Marcelo', testimonial:'Great work!'},
        {name: 'Juan Paco', testimonial:'Beautiful designs!'},
        {name: 'Pedro', testimonial:'Innovative!'},
    ],
 }),
}
</script>

<style>

</style>