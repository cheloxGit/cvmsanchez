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
            </v-avatar >
                {{about_me_label}}
            </v-chip>
        </v-card-title>
        <v-card-text>
            <v-row
                key="ab1"
                class="mb-6"
                no-gutters
            >
            <v-col
                key="ab2"
                class="text-left"
            >
                <v-card
                    class="pa-2"
                >
                    {{about_me}}
                </v-card>
            </v-col>
            <v-divider
                class="mx-4"
                vertical
            ></v-divider>
            <v-col
                key="ab3"
                class="text-left"
            >
                <!-- FactsAboutMe -->
                <FactsAboutMe
                    v-for="(fact, i) in facts_about_me"
                    :key="i"
                    :label="fact.label" 
                    :desc="fact.desc" 
                />
            </v-col>
            </v-row>
        </v-card-text>
    </div>
</template>

<script>
import FactsAboutMe from './about-me/FactsAboutMe.vue';

export default {
    name: "AboutMe",
    components: {
        FactsAboutMe
    },
    data: () => ({
        usr_name: 'Marcelo Sanchez Salazar',
        professional_degree: 'Systems Engineer',
        about_me: 'My name is Marcelo Sanchez Salazar, Freelancer. I have rich experience in web site design and building and customization, also I am good at wordpress. I love to talk with you about our unique.',
        facts_about_me: [
            {label:'Age ..............',desc:'............ 39'},
            {label:'Residence ...',desc:'...... Bolivia'},
            {label:'Freelance .....',desc:'... Available'},
        ],
        about_me_label: 'About Me',
    })
}
</script>

<style>
</style>