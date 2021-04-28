<template>
  <v-card>
    <v-card-title>
      User's
      <v-spacer></v-spacer>
      <v-text-field
        v-model="search"
        append-icon="mdi-magnify"
        label="Search"
        single-line
        hide-details
      ></v-text-field>
    </v-card-title>
    <v-data-table
      :headers="headers"
      :items="data"
      :search="search"
    ></v-data-table>
  </v-card>
</template>

<script>
  export default {
    data () {
      return {
        search: '',
        headers: [
          {
            text: 'Name',
            align: 'start',
            sortable: false,
            value: 'name',
          },
          { text: 'Email', value: 'email' },
          { text: 'Documents', value: 'documents' },
          { text: 'Sign', value: 'sign' },
          { text: 'XYZ', value: 'xyz' },
          { text: 'ABC', value: 'abc' },
        ],
        data: [
          {
            name: 'Ahmed',
            email: 201,
            documents: 5.0,
            sign: 34,
            xyz: 5.5,
            abc: '1.5%'
          },
          {
            name: 'Ali',
            email: 201,
            documents: 5.0,
            sign: 34,
            xyz: 5.5,
            abc: '1.5%'
          },
          {
            name: 'Faaiz',
            email: 201,
            documents: 5.0,
            sign: 34,
            xyz: 5.5,
            abc: '1.5%'
          },
          {
            name: 'Musa',
            email: 201,
            documents: 5.0,
            sign: 34,
            xyz: 5.5,
            abc: '1.5%'
          },
          {
            name: 'Hassan',
            email: 201,
            documents: 5.0,
            sign: 34,
            xyz: 5.5,
            abc: '1.5%'
          },
          {
            name: 'Ibrahim',
            email: 201,
            documents: 5.0,
            sign: 34,
            xyz: 5.5,
            abc: '1.5%'
          },
          {
            name: 'Adnan',
            email: 201,
            documents: 5.0,
            sign: 34,
            xyz: 5.5,
            abc: '1.5%'
          },
          {
            name: 'Awais',
            email: 201,
            documents: 5.0,
            sign: 34,
            xyz: 5.5,
            abc: '1.5%'          },
          {
            name: 'Habib',
            email: 201,
            documents: 5.0,
            sign: 34,
            xyz: 5.5,
            abc: '1.5%'
          },
          {
            name: 'Noor',
            email: 201,
            documents: 5.0,
            sign: 34,
            xyz: 5.5,
            abc: '1.5%' }
        ],
      }
    },
  }
</script>