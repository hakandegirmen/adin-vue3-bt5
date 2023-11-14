<script setup>
import NavBarVue from './components/NavBar.vue'
</script>
<script>
export default {
  components: {
    NavBarVue
  }
}
</script>
<template>
  <NavBarVue></NavBarVue>

  <RouterView />
</template>

<style scoped></style>
