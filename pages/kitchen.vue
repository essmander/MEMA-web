<template>
  <v-app id="inspire">
    <v-main>
      <v-container>
        <v-row>
          <v-col v-for="n in 24" :key="n" cols="4">
            <v-hover v-slot="{ hover }">
              <v-card
                :elevation="hover ? 12 : 2"
                class="mx-auto"
                height="350"
                max-width="350"
              >
                <v-card-text class="my-4 text-center text-h6">
                  Pickture
                </v-card-text>
              </v-card>
            </v-hover>
            <!-- <v-card height="200"></v-card> -->
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
}
</script>
