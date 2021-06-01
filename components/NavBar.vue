<template>
  <div>
    <b-navbar toggleable="lg" type="light">
      <b-navbar-brand href="#">
        <img
          class="logo"
          src="~assets/images/spotknacklogo.png"
          @click="openHomepage()"
        />
      </b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-auto">
          <NuxtLink to="/About" class="navbar-link"> About </NuxtLink>
          <NuxtLink to="/About" class="navbar-link"> Mission 2021 </NuxtLink>
          <NuxtLink to="/About" class="navbar-link"> Login </NuxtLink>
          <NuxtLink to="/About" class="navbar-link"> Signup </NuxtLink>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>
<script>
export default {
  methods: {
    openHomepage() {
      this.$router.push('/')
    },
  },
}
</script>
<style scoped>
.NuxtLogo {
  animation: 1s appear;
  margin: auto;
}

@keyframes appear {
  0% {
    opacity: 0;
  }
}
</style>
