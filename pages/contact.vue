<template>
  <ul style="list-style-type: none">
    <li v-for="worker in workers" :key="worker">
      <v-card class="mx-auto" max-width="900" outlined>
        <v-list-item three-line>
          <v-list-item-content>
            <div class="text-overline mb-4">OVERLINE</div>
            <v-list-item-title class="text-h5 mb-1">
              {{ worker.name }}
            </v-list-item-title>
            <v-list-item-subtitle>
              Email: {{ worker.email }}
              </v-list-item-subtitle>
              <v-list-item-subtitle>
              Tel: {{ worker.phone }}
              </v-list-item-subtitle>
          </v-list-item-content>
          <v-list-item-avatar tile size="80" color="grey"></v-list-item-avatar>
        </v-list-item>
      </v-card>
    </li>
  </ul>
</template>

<script>
export default {
  data () {
    return {
      workers: [
        {
          picture: 'mdi-apps',
          name: 'Viktor Björk',
          title: 'Snickare',
          email: '/',
          phone: '070-000 00 00'
        },
        {
          picture: 'mdi-apps',
          name: 'Christofer',
          title: 'Snickare',
          email: '/',
          phone: '070-000 00 00'
        }
      ]
    }
  }
}
</script>
