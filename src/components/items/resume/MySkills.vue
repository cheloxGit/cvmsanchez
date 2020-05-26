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
                {{myskills_label}}
            </v-chip>
        </v-card-title>
        <v-card-text>
            <!-- Row 1 -->
            <v-row
                key="ms1"
                class="mb-6"
                no-gutters
            >
            <!-- Resume: Experience -->
            <v-col
                key="ms2"
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
                    <v-icon>mdi-billboard</v-icon>
                    </v-avatar>
                        {{design_label}}
                </v-chip>
                </v-card-title>
                <v-card-text>
                <!-- Resume: LinearSkills -->
                <LinearSkills 
                    v-for="(linear_skill, i) in linear_skills"
                    :key="i"
                    :linear_skill="linear_skill.name" 
                    :percent_val="linear_skill.percent_val"
                />
                </v-card-text>
                </v-card>
            </v-col>
            <v-divider
                class="mx-4"
                vertical
            ></v-divider>
            <!-- MySkills: Language -->
            <v-col
                key="ms6"
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
                    <v-icon>mdi-flag-variant</v-icon>
                    </v-avatar>
                        {{language_label}}
                </v-chip>
                </v-card-title>
                <v-card-text>
                <!-- LanguageSkills -->
                    <LanguageSkills  
                        v-for="(language_skill, i) in language_skills"
                        :key="i"
                        :language="language_skill.language" 
                        :rating="language_skill.rating"
                    />
                </v-card-text>
                </v-card>
            </v-col>
            </v-row>
            <!-- CODING AND KNOWLEDGE -->
            <!-- Row 2 -->
            <v-row
                key="ms11"
                class="mb-6"
                no-gutters
            >
            <!-- Resume: Experience -->
            <v-col
                key="ms12"
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
                    <v-icon>mdi-code-tags</v-icon>
                    </v-avatar>
                        {{coding_label}}
                </v-chip>
                </v-card-title>
                <v-card-text>
                <!-- CodingSkills -->
                <CodingSkills 
                    v-for="(coding_skill, i) in coding_skills"
                    :key="i"
                    :number_one="coding_skill.number_one" 
                    :label_one="coding_skill.label_one"
                    :number_two="coding_skill.number_two" 
                    :label_two="coding_skill.label_two"
                />
                </v-card-text>
                </v-card>
            </v-col>
            <!-- Resume: Education -->
            <v-col
                key="ms25"
                class="text-center"
            >
                <v-card
                class="text-left"
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
                    <v-icon>mdi-codepen</v-icon>
                    </v-avatar>
                        {{knowledge_label}}
                </v-chip>
                </v-card-title>
                <v-card-text>
                    <KnowledgeSkills 
                        v-for="(knowledge_skill, i) in knowledge_skills"
                        :key="i"
                        :label="knowledge_skill.label" 
                    />
                </v-card-text>
                </v-card>
            </v-col>
            </v-row>
        </v-card-text>
  </div>
</template>

<script>
import LinearSkills from './LinearSkills.vue';
import LanguageSkills from './LanguageSkills.vue';
import CodingSkills from "./CodingSkills.vue";
import KnowledgeSkills from "./KnowledgeSkills.vue";

export default {
    name: "MySkills",
    components: {
        LinearSkills,
        LanguageSkills,
        CodingSkills,
        KnowledgeSkills
    },
    data () {
        return {
        myskills_label: 'My Skills',
        design_label: 'DESIGN',
        linear_skills: [
            {name:  'Web Design', percent_val: '80'},
            {name:  'Backend Services', percent_val: '60'},
            {name:  'Flutter', percent_val: '50'},
        ],
        language_label: 'LANGUAGES',
        language_skills: [
            {language:  'English', rating: '8'},
            {language:  'Spanish', rating: '10'},
        ],
        coding_label: 'CODING',
        coding_skills: [
            {number_one: '65', label_one: 'Node.js',number_two: '35', label_two: 'Python'},
            {number_one: '65', label_one: 'Vue.js', number_two: '35', label_two: 'Flutter'},
        ],
        knowledge_skills: [
            {label: 'Website hosting'},
            {label: 'Android and iOS apps'},
            {label: 'Arduino and Raspberry Pi Dev'},
        ],
        knowledge_label: 'KNOWLEDGE',
        knowledge_check_one: 'Website hosting',
        knowledge_check_two: 'Android and iOS apps',
        knowledge_check_three: 'Arduino and Raspberry Pi Dev',
        dense: true,
        inset: true,
     }}
}
</script>

<style>

</style>