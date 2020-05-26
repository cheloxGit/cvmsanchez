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
        ></v-avatar>{{resume_label}}
        </v-chip>
    </v-card-title>
    <v-card-text>
        <!-- Row 1 -->
        <v-row
            key="rm1"
            class="mb-6"
            no-gutters
        >
        <!-- Resume: Experience -->
        <v-col
            key="rm2"
            class="text-center"
        >
            <v-card
                class="center"
                max-width="200"
            >
            <v-card-title>
            <v-chip
                color="gray"
                label
            >
                <v-avatar
                    left
                    class="gray"
                >
                <v-icon>mdi-briefcase</v-icon>
                </v-avatar>
                    {{experience_label}}
            </v-chip>
            </v-card-title>
            <v-card-text>
            <v-divider inset="inset"></v-divider>
            <v-row
                key="rm3"
                class="mb-1 left"
                no-gutters
            >
            <v-chip
                class="mt-3"
                label
                color="green"
                outlined
            >{{experience_lapse_final}}</v-chip>
            </v-row>
            <v-row
                key="rm4"
                class="mt-1 pt-2 text-left"
                no-gutters
            >
                {{experience_lapse_final_position}}
            </v-row>
            <v-row
                key="rm5"
                no-gutters
            >
                {{experience_lapse_final_title}}
            </v-row>
            <v-row
                key="rm6"
                class="mt-1 pt-2 text-left"
                no-gutters
            >
                {{experience_lapse_final_desc}}
            </v-row>
            <v-divider inset="inset"></v-divider>
            <v-row
                key="rm7"
                class="mb-1 left"
                no-gutters
            >
            <v-chip
                class="mt-3"
                label
                color="gray"
                outlined
            >
                {{experience_lapse_intermediate}}
            </v-chip>
            </v-row>
            <v-row
                key="rm8"
                class="mt-1 pt-2 text-left"
                no-gutters
            >
                {{experience_lapse_intermediate_position}}
            </v-row>
            <v-row
                key="rm9"
                no-gutters
            >
                {{experience_lapse_intermediate_title}}
            </v-row>
            <v-row
                key="rm10"
                class="mt-1 pt-2 text-left"
                no-gutters
            >
                {{experience_lapse_intermediate_desc}}
            </v-row>
            </v-card-text>
            </v-card>
        </v-col>
        <v-divider
            class="mx-4"
            vertical
        ></v-divider>
        <!-- Resume: Education -->
        <v-col
            key="rm11"
            class="text-center"
        >
            <v-card
                class="center"
                max-width="200"
            >
            <v-card-title>
            <v-chip
                color="gray"
                label
            >
                <v-avatar
                    left
                    class="gray"
                >
                <v-icon>mdi-school</v-icon>
                </v-avatar>
                    {{education_label}}
            </v-chip>
            </v-card-title>
            <v-card-text>
            <v-divider inset="inset"></v-divider>
            <v-row
                key="rm12"
                class="mb-1 left"
                no-gutters
            >
            <v-chip
                class="mt-3"
                label
                color="gray"
                outlined
            >
                {{education_lapse_final}}
            </v-chip>
            </v-row>
            <v-row
                key="rm13"
                class="mt-1 pt-2 text-left"
                no-gutters
            >
                {{education_lapse_final_institution}}
            </v-row>
            <v-row
                key="rm14"
                no-gutters
            >
                {{education_lapse_final_title}}
            </v-row>
            <v-row
                key="rm15"
                class="mt-1 pt-2 text-left"
                no-gutters
            >
                {{education_lapse_final_desc}}
            </v-row>
            <v-divider inset="inset"></v-divider>
            <v-row
                key="rm16"
                class="mb-1 left"
                no-gutters
            >
            <v-chip
                class="mt-3"
                label
                color="gray"
                outlined
            >
                {{education_lapse_intermediate}}
            </v-chip>
            </v-row>
            <v-row
                key="rm17"
                class="mt-1 pt-2 text-left"
                no-gutters
            >
                {{education_lapse_intermediate_institution}}
            </v-row>
            <v-row
                key="rm18"
                no-gutters
            >
                {{education_lapse_intermediate_title}}
            </v-row>
            <v-row
                key="rm19"
                class="mt-1 pt-2 text-left"
                no-gutters
            >
                {{education_lapse_intermediate_desc}}
            </v-row>
            </v-card-text>
            </v-card>
        </v-col>
        </v-row>
    </v-card-text>
  </div>
</template>

<script>
export default {
    name: "Resume",
     data: () => ({
        resume_label: 'Resume',
        experience_label: 'Experience',
        experience_lapse_final: '2017 - Present',
        experience_lapse_final_position: 'CEO',
        experience_lapse_final_title: 'Nine Brains Corp.',
        experience_lapse_final_desc: 'Collaborate with creative and development teams on the execution of ideas.',
        experience_lapse_intermediate: '2010 - 2018',
        experience_lapse_intermediate_position: 'Developer',
        experience_lapse_intermediate_title: 'Viva D.R.',
        experience_lapse_intermediate_desc: 'Worked in Viva Republica Dominicana, areas Datawarehouse, DevOps, OracleSQL, PHP, PLSQL.',
        education_label: 'Education',
        education_lapse_final: ' 2010 - 2018',
        education_lapse_final_institution: 'UMSS',
        education_lapse_final_title: 'Engineer System',
        education_lapse_final_desc: 'Time studying in UMSS and knowledge',
        education_lapse_intermediate: '2010 - 2018',
        education_lapse_intermediate_institution: 'Developer',
        education_lapse_intermediate_title: 'Viva D.R.',
        education_lapse_intermediate_desc: 'Worked in Viva Republica Dominicana, areas Datawarehouse, DevOps, OracleSQL, PHP, PLSQL.',
        inset: true,
     })
}
</script>

<style>

</style>