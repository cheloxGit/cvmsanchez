<template>
    <v-card
        max-width="350"
        tile
    >
        <v-img
            height="600"
            :src="url_image_bg"
        >
        <v-row
        align="end"
        class="fill-height"
        >
            <v-col
                align-self="end"
                class="pa-0"
                cols="12"
            >
                <v-avatar
                    class="profile"
                    color="grey"
                    size="164"
                >
                    <v-img :src="url_image_profile"></v-img>
                </v-avatar>
            </v-col>
            <v-col class="py-0">
                <v-list-item
                    color="rgba(0, 0, 0, .4)"
                    dark
                >
                    <v-list-item-content>
                        <v-list-item-title class="title">{{usr_name}}</v-list-item-title>
                        <v-list-item-subtitle>{{professional_degree}}</v-list-item-subtitle>
                    </v-list-item-content>
                </v-list-item>
        </v-col>
        </v-row>
        </v-img>
    </v-card>
</template>


<script>
export default {
  name: "Avatar",

  data: () => ({
    usr_name: 'Marcelo Sanchez Salazar',
    url_image_bg: 'https://bslthemes.com/ryan/demo/images/bg.jpg',
    url_image_profile: 'https://bslthemes.com/ryan/demo/images/profile.png',
    professional_degree: 'Systems Engineer',
  })
};
</script>
