<template>
    <v-app>
        <v-app-bar app color="primary" dark>
            <v-spacer></v-spacer>

            <v-btn href="https://github.com/vuetifyjs/vuetify/releases/latest" target="_blank" text> </v-btn>
        </v-app-bar>

        <v-main>
            <v-row justify="center">
                <v-col cols="6">
                    <div class="text-center">
                        <v-btn @click="changeText()">
                            Click me
                        </v-btn>
                    </div>
                </v-col>
            </v-row>
            <v-row justify="center">
                <v-col cols="4" class="text-center">
                    {{ text }}
                </v-col>
            </v-row>
        </v-main>
    </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld';

export default {
    name: "App",

    components: {
        //HelloWorld,
    },

    data: () => ({
        text: "Hello Max!",
    }),

    methods: {
        changeText() {
            this.text = "Hello Louis";
        },
    },
};
</script>
