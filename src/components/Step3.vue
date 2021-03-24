<template>
    <div>
        <center>
        <br><br><h2>Напиши что-нибудь о себе</h2><br><br>
        <v-text-field class="vInput"
                v-model="FirstName"
                label="About myself"
                placeholder="">
            </v-text-field>
        </center>
        <v-img
:aspect-ratio="16/9"
:width="width"
src="https://images.unsplash.com/photo-1508583732154-e9ff899f8534?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=700&q=80"
></v-img>
        <br><br>
    </div>
</template>