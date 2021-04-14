<template>
  <div class="label" :style="style">{{ text }}</div>
</template>

<script>
export default {
  name: 'Label',
  props: {
    text: {
      type: String,
      default: '',
    },
    background: {
      type: String,
      default: null,
    },
    crossed: {
      type: Boolean,
      default: false,
    },
    color: {
      type: String,
      default: null,
    },
  },
  computed: {
    style() {
      return {
        background: this.background,
        'text-decoration': this.crossed ? 'line-through' : 'none',
        color: this.color,
      };
    },
  },
};
</script>

<style lang="scss" scoped>
.label {
  display: flex;
  justify-content: center;
  align-items: center;
  background: #cccbcb;
  width: 80px;
  height: 30px;
  color: #767676;
  border-radius: 30px;
}
</style>
