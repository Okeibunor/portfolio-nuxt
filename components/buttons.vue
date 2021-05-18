<template>
  <button :style="style" class="btn">
    {{ title }}
    <img v-if="image" :src="require(`~/assets/images/${image}.svg`)" alt="" />
  </button>
</template>

<script>
export default {
  name: "buttons",
  props: {
    title: String,
    color: String,
    background: String,
    image: String,
  },
  data: function () {
    return {
      style: {
        color: this.color,
        background: this.background,
      },
    };
  },
};
</script>

<style lang="scss" scoped>
.btn img {
  vertical-align: middle;
  margin: auto 0 auto 0.4rem;
}
.btn {
  padding: 0.6rem 1.3rem;
  border-radius: 0.55rem;
  border: 2.5px solid #2d9cdb;
  font-size: 1.5rem;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
</style>
