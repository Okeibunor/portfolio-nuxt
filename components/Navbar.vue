<template>
  <nav class="navbar">
    <img src="@/assets/images/logo.svg" alt="logo" />
    <ul class="navbar-items">
      <NuxtLink class="navbar-link" to="/">Home</NuxtLink>
      <NuxtLink class="navbar-link" to="/about">About Me</NuxtLink>
      <NuxtLink class="navbar-link" to="/portfolio">Portfolio</NuxtLink>
      <NuxtLink class="navbar-link" to="/resume">Resume</NuxtLink>
      <NuxtLink class="navbar-link" to="/mentor">Mentorship</NuxtLink>
    </ul>
    <buttons
      image="monkeyemoji"
      color="white"
      background="#2d9cdb"
      title="Talk to Me"
    />
  </nav>
</template>

<script>
import buttonBlue from "./buttons.vue";
export default {
  components: { buttonBlue },
  name: "Navbar",
};
</script>

<style lang="scss" scoped>
$font-colored: #2d9cdb;
$button-color: #2d9cdb;
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  margin: 3.5vh auto;
  padding: 0 5vw;
}
.navbar-items {
  display: flex;
  width: 44%;
  justify-content: space-between;
  align-items: center;

  .navbar-link {
    list-style-type: none;
    font-size: 1.4rem;
    text-decoration: none;
    color: black;
  }
}

.nuxt-link-exact-active {
  color: $font-colored !important;
}
</style>
