<template>
  <div>
    <Navbar />
    <p class="hero-vertical-container">Okeibunor Favour</p>

    <hero />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar";
import Hero from "../components/Hero.vue";
export default {
  name: "index",
  components: {
    Navbar,
    Hero,
  },
};
</script>

<style lang="sass" scoped>
.hero-vertical-container
  display: flex
  align-items: center
  writing-mode: vertical-rl
  font-size: 11px
  line-height: 13px
  letter-spacing: 2px
  color: #161616
  transform: rotate(-180deg)
  text-transform: uppercase
  z-index: 1
  text-transform: uppercase
  position: absolute
</style>
