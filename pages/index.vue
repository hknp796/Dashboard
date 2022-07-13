<template>
  <div>
    <nav-bar />
    <dash-board />
    <main-account />
  </div>
</template>

<script>
import mainAccount from '../components/main-account.vue'
export default {
  name: 'IndexPage',
  components: { mainAccount },
}
</script>
