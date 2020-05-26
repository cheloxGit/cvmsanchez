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
                {{my_services_label}}
            </v-chip>
        </v-card-title>
        <v-card-text>

        </v-card-text>
        <ServicesList 
            v-for="(service, i) in services_list"
            :key="i"
            :title_one="service.title_one" 
            :src_bg_one="service.src_bg_one"
            :subtitle_one="service.subtitle_one"
            :desc_one="service.desc_one"
            :title_two="service.title_two" 
            :src_bg_two="service.src_bg_two"
            :subtitle_two="service.subtitle_two"
            :desc_two="service.desc_two"
        />
    </div>
</template>

<script>
import ServicesList from './ServicesList.vue';

export default {
    name: "MyServices",
    components: {
        ServicesList
    },
    data: () => ({
        my_services_label: 'My Services',
        services_list: [
            {
                title_one:'Web Development', subtitle_one:'Vue.js', desc_one:'This CV was development under Vue.js. Here is the Product', src_bg_one:'https://cdn.vuetifyjs.com/images/cards/docks.jpg',
                title_two:'Mobile Hybrid Dev', subtitle_two:'Flutter', desc_two:'Recently work with Flutter to deploy.Here is the Product', src_bg_two:'https://cdn.vuetifyjs.com/images/cards/docks.jpg'
            },
            {
                title_one:'Python Developer', subtitle_one:'Python as Backservice', desc_one:'Python as Backservice Working on multiple projects with Python, Pandas, Requests, Selenium, API, etc. Here is the Product',src_bg_one:'https://cdn.vuetifyjs.com/images/cards/docks.jpg',
                title_two:'Robotics Dev', subtitle_two:'Arduino and Raspberry PI', desc_two:'Private works with Arduino, NodeMCU, Raspberry PI, GSM, CNC, Follow cars, etc. Here is the Product',src_bg_two:'https://cdn.vuetifyjs.com/images/cards/docks.jpg'
            },
        ],
    })
}
</script>

<style>

</style>