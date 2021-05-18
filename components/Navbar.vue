<template>
  <nav class="navbar">
    <img src="@/assets/images/logo.svg" alt="logo" />
    <ul class="navbar-items">
      <li class="active">Home</li>
      <li>About Me</li>
      <li>Portfolio</li>
      <li>Resume</li>
      <li>Mentorship</li>
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
}
.navbar-items {
  display: flex;
  width: 44%;
  justify-content: space-between;
  align-items: center;

  li {
    list-style-type: none;
    font-size: 1.4rem;

    &.active {
      color: $font-colored;
      &::after {
        content: "";
      }
    }
  }
}
</style>
