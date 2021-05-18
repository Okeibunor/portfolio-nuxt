<template>
  <div class="container">
    <Navbar />
    <!-- <p class="hero-vertical-container">Okeibunor Favour</p> -->
    <img src="~/assets/images/dots.svg" alt="dots" class="dots dots-left" />
    <img src="~/assets/images/dots.svg" alt="dots" class="dots dots-right" />
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
.container
  position: relative

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

.dots
  position: absolute
  bottom: 0

.dots-right
  right: 0

.dots-left
  left: 0
</style>
