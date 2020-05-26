<template>
<div>
    <v-divider inset="inset"></v-divider>
        <v-row
            key="ms7"
            class="mb-1 left"
            no-gutters
        >
            {{language}}
        </v-row>
        <v-row
            key="ms8"
            class="mb-1 left"
            no-gutters
        >
        <v-rating
            :value="rating"
            length="10"
            empty-icon="mdi-checkbox-blank-circle-outline"
            full-icon="mdi-checkbox-blank-circle"
            :readonly="true"
            size="16"
            dense="dense"
            background-color="grey darken-1"
            color="green"
        ></v-rating>
        </v-row>
    <v-divider inset="inset"></v-divider>
</div>
</template>

<script>
export default {
    name: "LanguageSkills",
    props: {
        language: String,
        rating: String,
    }
}
</script>

<style>

</style>