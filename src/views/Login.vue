<template>
    <div class="center">
        <v-row>
            <v-col cols="10" offset="1" sm="6" offset-sm="3" md="4" offset-md="4" >
                <v-avatar color="primary" size="95" tile>
                    <v-img src="@/assets/logo.png"></v-img>
                </v-avatar>
                <v-text-field label="Regular" placeholder="Placeholder" v-model="username"></v-text-field>
                <v-text-field label="Regular" placeholder="Placeholder" v-model="password" type="password"></v-text-field>
                <template>
                    <v-btn  class="base-inverted" block @click="authenticate()">
                        Login
                    </v-btn>
                </template>
            </v-col>
        </v-row>
    </div>
</template>

<script>
export default {
    data() {
        return {
            username: "",
            password: ""
        }
    },
    methods: {
        authenticate() {
            alert("login success")

        }
    },

}
</script>

<style lang="scss" scoped></style>