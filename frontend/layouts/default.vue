<template>
  <v-app>
    <v-app-bar fixed app>
      <v-spacer/>
        <v-toolbar-title> 
          <nuxt-link to="/">
            <v-btn icon plain :ripple="false" >
              <v-icon large>
                {{ mdiHomeVariant }}
              </v-icon>
            </v-btn>
          </nuxt-link>
        </v-toolbar-title>
      <v-spacer/>
    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer app>
      <v-spacer />
      <span>&copy; {{ new Date().getFullYear() }} Framework Guide</span>
      <v-spacer />
    </v-footer>
  </v-app>
</template>

<script>
import { mdiHomeVariant } from '@mdi/js'
export default {
  name: 'DefaultLayout',

  setup() {
    return { mdiHomeVariant }
  }
}
</script>
