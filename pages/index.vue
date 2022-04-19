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
import Faq from '../components/faq.vue'
export default { components: { Navbar, Team, Faq } }
</script>
