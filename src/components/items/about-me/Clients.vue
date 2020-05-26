<template>
<div>
    <!-- CLIENTS -->
    <v-card-title>
        <v-chip
            class="ma-2"
            color="green lighten-1"
            text-color="white"
        >
        <v-avatar
            left
            class="green darken-1"
        ></v-avatar>
            {{clients_label}}
        </v-chip>
    </v-card-title>
    <v-card-text>
        <!-- Row 1 -->
        <v-row
            key="cl1"
            no-gutters
        >
        <!-- Web Development -->
        <v-col
            key="cl2"
            class="text-center"
        >
            <v-card
                max-width="250"
            >
            <v-avatar
                size="250"
            ><v-img  height="100px" :src="clients_one_img_url"></v-img></v-avatar>
            </v-card>
        </v-col>
        <v-divider
            class="mx-4"
            vertical
        ></v-divider>
        <!-- Mobile Hybrid Development -->
        <v-col
            key="cl3"
            class="text-center"
        >
            <v-card>
                <v-avatar
                    size="250"
                ><v-img height="100px" :src="clients_two_img_url"></v-img></v-avatar>
            </v-card>
        </v-col>
        <v-col
            key="cl4"
            class="text-center"
        >
            <v-card>
                <v-avatar
                    size="250"
                ><v-img height="100px" :src="clients_one_img_url"></v-img></v-avatar>
            </v-card>
        </v-col>
       <v-col
            key="cl5"
            class="text-center"
        >
            <v-card>
                <v-avatar
                    size="250"
                ><v-img height="100px" :src="clients_one_img_url"></v-img></v-avatar>
            </v-card>
        </v-col>
        </v-row>
</v-card-text>  
</div> 
</template>

<script>
export default {
    name: "Clients",
    data: () => ({
        clients_label: 'Clients',
        clients_one_img_url: 'https://www.nerdsonsite.com/wp-content/uploads/2019/07/nerds-on-site-car@2x.png',
        clients_two_img_url: 'https://oneextraguy.com/wp-content/uploads/2017/02/logo.jpg',
    })
}
</script>

<style>

</style>