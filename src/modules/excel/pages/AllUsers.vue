<template>
    <v-container>
        <v-row class="text-center">
            <v-col cols="12">
                <h2>Mostrar usuarios</h2>
                <v-icon icon="mdi-vuetify"></v-icon>

            </v-col>
        </v-row>
    </v-container>
</template>

<script>
import axios from "axios";

export default {
    name: 'AllUsers',
    components: {
    },

    data: () => ({
        users: null
    }),

    created() {
        axios.get("18.224.73.103/api/users")
            .then((result) => {
                this.users = result;
            })
    }
}
</script>

<style></style>