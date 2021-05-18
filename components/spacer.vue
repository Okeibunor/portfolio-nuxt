<template>
  <div class="spacer" :style="styleObject"></div>
</template>

<script>
export default {
  name: "spacer",
  data: function () {
    return {
      styleObject: {
        width: `${this.width}rem`,
        height: `${this.height}rem`,
      },
    };
  },
  props: ["width", "height"],
};
</script>

<style lang="scss" scoped>
.spacer {
  margin: auto;
}
</style>
