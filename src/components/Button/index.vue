<template>
  <button :type="type">{{ text }}</button>
</template>
<script>
export default {
  name: "Button",
  props: {
    text: {
      type: String,
      default: "button",
    },
    type: {
      type: String,
      default: "button",
    },
  },
};
</script>
<style scoped lang="scss">
$sel: ".btn";
#{$sel} {
  padding: 10px 20px;
  border-radius: 10px;
  border: none;
  color: white;
  font-weight: bold;
  cursor: pointer;
  &#{$sel}-primary {
    background-color: $primary-color;
  }
  &#{$sel}-secondary {
    background-color: $primary-color-light-1;
  }
  &#{$sel}-danger {
    background-color: $primary-color-light-2;
  }
  &#{$sel}-warning {
    background-color: $primary-color-light-3;
  }
  &#{$sel}-success {
    background-color: $primary-color-dark-3;
  }
  &#{$sel}-info {
    background-color: $primary-color-light-1;
  }
  &:hover {
    opacity: 0.8;
    background-color: white;
    color: $primary-color;
    border: 1px solid black;
  }
}
</style>
