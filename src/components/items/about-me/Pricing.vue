<template>
  <div>
        <!-- PRICING -->
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
                {{pricing_label}}
            </v-chip>
        </v-card-title>

        <v-card-text>
            <!-- Row 1 -->
            <v-row
                key="1"
                class="mb-6"
                no-gutters
            >
            <!-- Web Development -->
            <v-col
                key="2"
                class="text-left"
            >
                <v-card
                    class="text-center"
                    max-width="200"
                >
                <v-icon >mdi-speedometer-slow</v-icon>
                <v-card-subtitle class="pb-0">{{pricing_basic_label}}</v-card-subtitle>
                <v-card-text class="text--primary">
                <v-row align="center">
                <v-col class="display-1" cols="18">
                <v-badge
                    class="pr-2"
                    bordered
                    color="green"
                    icon="mdi-currency-usd"
                    overlap
                    right
                >{{pricing_basic_number}}</v-badge>
                    {{pricing_lapse}}
                </v-col>
                </v-row>
                <div>{{pricing_basic_one}}</div>
                <div>{{pricing_basic_two}}</div>
                <div>{{pricing_basic_three}}</div>
                <div>{{pricing_basic_four}}</div>
                <div>{{pricing_basic_five}}</div>
                </v-card-text>
                <v-card-actions>
                    <v-btn
                        color="orange"
                        text
                    >{{pricing_basic_label_buy}}</v-btn>
                </v-card-actions>
                </v-card>
            </v-col>
            <v-divider
                class="mx-4"
                vertical
            ></v-divider>
            <!-- Mobile Hybrid Development -->
            <v-col
                key="3"
                class="text-left"
            >
                <v-card
                    class="text-center"
                    max-width="200"
                >
                <v-icon >mdi-speedometer</v-icon>
                <v-card-subtitle class="pb-0">{{pricing_pro_label}}</v-card-subtitle>
                <v-card-text class="text--primary">
                <v-row align="center">
                <v-col class="display-1" cols="18">
                    <v-badge
                        class="pr-2"
                        bordered
                        color="green"
                        icon="mdi-currency-usd"
                        overlap
                        right
                    >{{pricing_pro_number}}</v-badge>
                        {{pricing_lapse}}
                </v-col>
                </v-row>
                <div>{{pricing_pro_one}}</div>
                <div>{{pricing_pro_two}}</div>
                <div>{{pricing_pro_three}}</div>
                <div>{{pricing_pro_four}}</div>
                <div>{{pricing_pro_five}}</div>
                </v-card-text>
                <v-card-actions>
                    <v-btn
                        color="orange"
                        text
                    >{{pricing_pro_label_buy}}</v-btn>
                </v-card-actions>
                </v-card>
            </v-col>
            </v-row>
        </v-card-text>
  </div>
</template>

<script>
export default {
    name: "Pricing",
    data: () => ({
        pricing_label: 'Pricing',
        pricing_basic_label: 'Basic',
        pricing_basic_number: '15',
        pricing_lapse: 'hour',
        pricing_basic_one: 'Web Development',
        pricing_basic_two: 'Advertising',
        pricing_basic_three: 'Game Development',
        pricing_basic_four: 'Music Writing',
        pricing_basic_five: 'Photography',
        pricing_basic_label_buy: 'BUY BASIC',
        pricing_pro_label: 'Pro',
        pricing_pro_number: '20',
        pricing_pro_one: 'Web Development',
        pricing_pro_two: 'Advertising',
        pricing_pro_three: 'Game Development',
        pricing_pro_four: 'Music Writing',
        pricing_pro_five: 'Photography',
        pricing_pro_label_buy: 'BUY PRO',
        
    })
}
</script>

<style>

</style>