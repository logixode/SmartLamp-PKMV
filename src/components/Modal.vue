<template>
  <v-row justify="center">
    <v-dialog v-model="dialog" persistent max-width="600px">
      <v-card class="pa-3">
        <slot></slot>

        <!-- <v-card-title>
          <span class="headline">Title</span>
        </v-card-title>
        <v-card-text>
          <v-container>
            <v-row>
              <v-col cols="12">
                <v-text-field label="SSID" required></v-text-field>
              </v-col>
              <v-col cols="12">
                <v-text-field
                  label="Password"
                  type="password"
                  required
                ></v-text-field>
              </v-col>
            </v-row>
          </v-container>
        </v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn color="blue darken-1" text @click="dialog = false">
            Close
          </v-btn>
          <v-btn color="blue darken-1" text @click="dialog = false">
            Save
          </v-btn>
        </v-card-actions> -->
      </v-card>
    </v-dialog>
  </v-row>
</template>

<script>
export default {
  data: () => ({}),
  computed: {
    dialog() {
      return this.$store.state.modalEditColor;
    }
  }
};
</script>

<style>
</style>