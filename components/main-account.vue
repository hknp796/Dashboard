<template>
  <div class="wrapper d-flex pa-9 mx-4">
    <div class="mr-9">
      <h3 class="mb-6">Main Account</h3>
      <h1>$ 280,820 <small class="subtitle-1">(USD)</small></h1>
      <p>From 20 Jan,2022-20 Feb,2022</p>
      <v-btn color="#2666EB" class="white--text" rounded height="45">
        Withdraw</v-btn
      >
      <v-btn color="grey" rounded height="45">Link Account</v-btn>
    </div>
    <div>
      <v-card
        class="mx-auto card white--text"
        max-width="344"
        outlined
        color="#2666EB"
      >
        <v-list-item three-line>
          <v-list-item-content class="white--text">
            <div>Primary Card</div>
            <h5 class="mb-4">See All Card</h5>
            <v-list-item-subtitle class="white--text"
              >1234 1233 4455 6764</v-list-item-subtitle
            >
          </v-list-item-content>

          <v-list-item-avatar tile size="80" color="grey"></v-list-item-avatar>
        </v-list-item>

        <v-card-actions>
          <p>Barely vanduito</p>
        </v-card-actions>
      </v-card>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      amount: 280820,
    }
  },
}
</script>

<style scoped>
.wrapper {
  border: 1px solid grey;
  border-radius: 10px;
  width: max-content;
}

.card {
  border-radius: 20px;
}
</style>
