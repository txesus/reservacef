<template>
  <v-container>
    <v-row class="text-center">

      <v-col cols="12">
        <h1 class="display-2 font-weight-bold mb-3">
          Formulario de la CEF
        </h1>
      </v-col>
      <v-col cols="12">
        <v-form @submit.prevent>
        <v-col sm="6">
          <v-text-field
            v-model="firstName"
            :rules="rules"
            label="Nombre"
          ></v-text-field>
        </v-col>
        <v-col sm="6">
          <v-text-field
            v-model="firstName"
            :rules="rules"
            label="Apellidos"
          ></v-text-field>
        </v-col>
        <v-col sm="6">
          <v-text-field
            v-model="firstName"
            :rules="rules"
            label="Teléfono"
          ></v-text-field>
        </v-col>
        <v-col sm="6">
          <v-text-field
            v-model="email"
            :rules="emailRules"
            label="E-mail"
            hide-details
            required
          ></v-text-field>
        </v-col>
        <v-col sm="6">
          <v-date-picker></v-date-picker>
        </v-col>
        <v-col sm="6">
          <v-select
            label="Dias que necesitas hotel"
            :items="['Jueves', 'Viernes', 'Sábado']"
            multiple
            variant="outlined"
          ></v-select>
        </v-col>
        <v-btn class="mt-2" type="submit" block>Enviar</v-btn>
      </v-form>
      
      </v-col>


    </v-row>
  </v-container>
</template>

<script>

export default {
  name: 'HelloWorld',

  data: () => ({
    ecosystem: [
      {
        text: 'vuetify-loader',
        href: 'https://github.com/vuetifyjs/vuetify-loader/tree/next',
      },
      {
        text: 'github',
        href: 'https://github.com/vuetifyjs/vuetify/tree/next',
      },
      {
        text: 'awesome-vuetify',
        href: 'https://github.com/vuetifyjs/awesome-vuetify',
      },
    ],
    importantLinks: [
      {
        text: 'Chat',
        href: 'https://community.vuetifyjs.com',
      },
      {
        text: 'Made with Vuetify',
        href: 'https://madewithvuejs.com/vuetify',
      },
      {
        text: 'Twitter',
        href: 'https://twitter.com/vuetifyjs',
      },
      {
        text: 'Articles',
        href: 'https://medium.com/vuetify',
      },
    ],
    whatsNext: [
      {
        text: 'Explore components',
        href: 'https://vuetifyjs.com',
      },
      {
        text: 'Roadmap',
        href: 'https://vuetifyjs.com/introduction/roadmap/',
      },
      {
        text: 'Frequently Asked Questions',
        href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
      },
    ],
  }),
}
</script>
