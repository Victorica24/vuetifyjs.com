<template>
  <v-container fluid>
    <v-layout row>
      <v-flex xs4>
        <v-subheader>Normal with hint text</v-subheader>
      </v-flex>
      <v-flex xs8>
        <v-text-field
          name="input-1-3"
          label="Hint Text"
          single-line
        ></v-text-field>
      </v-flex>
    </v-layout>
    <v-layout row>
      <v-flex xs4>
        <v-subheader>Press</v-subheader>
      </v-flex>
      <v-flex xs8>
        <v-text-field
          name="input-2-3"
          label="Hint Text"
          class="input-group--focused"
          single-line
        ></v-text-field>
      </v-flex>
    </v-layout>
    <v-layout row>
      <v-flex xs4>
        <v-subheader>Focus</v-subheader>
      </v-flex>
      <v-flex xs8>
        <v-text-field
          name="input-3-3"
          label="Hint Text"
          value="Input text"
          class="input-group--focused"
          single-line
        ></v-text-field>
      </v-flex>
    </v-layout>
    <v-layout row>
      <v-flex xs4>
        <v-subheader>Normal with input text</v-subheader>
      </v-flex>
      <v-flex xs8>
        <v-text-field
          name="input-3-4"
          label="Hint Text"
          value="Input text"
          single-line
        ></v-text-field>
      </v-flex>
    </v-layout>
    <v-layout row>
      <v-flex xs4>
        <v-subheader>Error</v-subheader>
      </v-flex>
      <v-flex xs8>
        <v-text-field
          :rules="[() => 'Username or Password is incorrect.']"
          name="input-3-5"
          label="Hint Text"
          value="Input text"
          error
          single-line
        ></v-text-field>
      </v-flex>
    </v-layout>
    <v-layout row>
      <v-flex xs4>
        <v-subheader>Disabled</v-subheader>
      </v-flex>
      <v-flex xs8>
        <v-text-field
          name="input-3"
          label="Label Text"
          value="Input text"
          disabled
          single-line
        ></v-text-field>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
  export default {
    data () {
      return {
        rules: [
          () => 'Username or Password is incorrect'
        ]
      }
    }
  }
</script>
