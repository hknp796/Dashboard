<template>
  <div>
    <div class="d-flex wrappers align-center px-3">
      <v-col sm="2">
        <v-text-field
          outlined
          prepend-inner-icon="mdi-magnify"
          placeholder="Search a Transaction"
          hide-details="true"
        >
        </v-text-field>
      </v-col>
      <div class="d-flex align-center">
        <v-btn outlined color="blue" rounded>Basic Plan</v-btn>
        <v-btn icon class="mx-5">
          <v-icon>mdi-bell</v-icon>
        </v-btn>
        <v-avatar>
          <img src="https://cdn.vuetifyjs.com/images/john.jpg" alt="John" />
        </v-avatar>
      </div>
    </div>
    <v-divider></v-divider>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.wrappers {
  justify-content: space-between;
}
</style>
