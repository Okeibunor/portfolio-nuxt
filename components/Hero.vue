<template>
  <div class="hero">
    <spacer :width="4" :height="3" />
    <div class="hero-medium-container">
      <img src="~/assets/images/hand.svg" alt="hand" class="wave" />
      <span class="hero-text">
        <img src="~/assets/images/star.svg" alt="star" class="star" />
        , I’m Okeibunor Favour

        <img
          src="~/assets/images/concave.svg"
          alt="concave"
          class="concave animate__animated animate__wobble"
        />
      </span>
    </div>
    <spacer :width="4" :height="3" />
    <vue-typer
      :text="[
        'Frontend Engineer',
        'Fullstack Web Developer',
        'Blockchain Enthusiast',
        'Drummer boy...',
      ]"
      :repeat="Infinity"
      :shuffle="false"
      initial-action="typing"
      :pre-type-delay="150"
      :type-delay="100"
      :pre-erase-delay="2000"
      :erase-delay="1000"
      erase-style="select-all"
      :erase-on-complete="false"
      caret-animation="blink"
    ></vue-typer>
    <spacer :width="4" :height="3" />
    <div class="btn-group">
      <buttons
        image="monkeyemoji"
        color="#2D9CDB"
        background="white"
        title="Talk to Me"
      /><spacer :width="1" :height="0" />
      <buttons
        image="github"
        background="#2D9CDB"
        color="white"
        title="Projects"
      />
    </div>
    <spacer :width="1" :height="3.7" />
    <img style="width: 84%" src="~/assets/images/waves.svg" alt="" />
  </div>
</template>

<script>
import ButtonBlue from "./buttons.vue";
import spacer from "./spacer.vue";
export default {
  components: { spacer, ButtonBlue },
  name: "hero",
};
</script>

<style lang="scss" scoped>
.hero {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.hero-medium-container {
  display: flex;
  justify-content: center;
  align-items: center;
}
.wave {
  animation: wave 0.75s ease-in-out infinite alternate-reverse;

  @keyframes wave {
    from {
      transform: rotate(7deg);
      transform-origin: 100% 100%;
    }
    to {
      transform: rotate(-7deg);
      transform-origin: 100% 100%;
    }
  }
}
.hero-text {
  font-weight: 700;
  font-size: 4.7rem;
  line-height: 5.2rem;
  position: relative;
}

.concave {
  position: absolute;
  right: 1rem;
  bottom: -2rem;
}
.star {
  position: absolute;
  right: -2rem;
  top: -1.5rem;
}
.btn-group {
  display: flex;
}
</style>
