<template>
<div>
    <v-divider inset="inset"></v-divider>
    <v-row
        key="ms3"
        class="mb-1 left"
        no-gutters
    >
        {{linear_skill}}
    <v-progress-linear color="green" :value="percent_val"></v-progress-linear>
    </v-row>
    <v-divider inset="inset"></v-divider>
</div>
    
</template>

<script>
export default {
    name: "LinearSkills",
    props: {
        linear_skill: String,
        percent_val: String
    }
}
</script>

<style>

</style>