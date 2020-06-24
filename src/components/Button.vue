<template>
  <button
    id="mk-btn"
    :class="classess"
  >
    <slot />
  </button>
</template>

<script>
export default {
  name: 'ju-btn',
  props: {
    rounded: {
      type: Boolean,
      default: false,
    },
    color: {
      type: String,
      default: '',
    },
    customClass: {
      type: String,
      default: '',
    },
  },
  computed: {
    classess() {
      return [
        `${this.rounded ? 'rounded' : null}`,
        `${this.color ? this.color : 'bg-gray-100'}`,
        `${this.customClass ? this.customClass : null}`,
      ];
    },
  },
};
</script>

<style lang="scss">

</style>
