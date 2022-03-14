<template>
  <div>
    <Navbar />
    <Team />
    <Faq />
  </div>
</template>

<script>
import Navbar from '../components/navbar.vue'
import Team from '../components/team.vue'
export default { components: { Navbar, Team } }
</script>
