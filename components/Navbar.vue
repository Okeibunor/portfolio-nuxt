<template>
  <nav class="navbar">
    <img src="@/assets/images/logo.svg" alt="" />
    <ul class="navbar-items">
      <li class="active">Home</li>
      <li>About Me</li>
      <li>Portfolio</li>
      <li>Resume</li>
      <li>Mentorship</li>
    </ul>
    <button class="btn">
      Talk to Me
      <img src="@/assets/images/monkeyemoji.svg" alt="" />
    </button>
  </nav>
</template>

<script>
export default {
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
  margin: 5vh auto;
  font-size: 1.5rem;
}
.navbar-items {
  display: flex;
  width: 45%;
  justify-content: space-between;
  align-items: center;

  li {
    list-style-type: none;
    &.active {
      color: $font-colored;
      &::after {
        content: "";
      }
    }
  }
}
.btn img {
  vertical-align: middle;
  margin: auto 0 auto 0.4rem;
}
</style>
