<template>
  <div class="main">
    <label for=""><i class="ri-shining-fill"></i> {{ label }}...</label>
    <input
      :type="type"
      :placeholder="placeholder"
      :value="modelValue"
      @input="$emit('input', $event.target.value)"
    />
  </div>
</template>
<script>
import Wrapper from "./../Dashboard/index.vue";
export default {
  name: "Input",
  props: {
    type: {
      type: String,
      default: "text",
    },
    placeholder: {
      type: String,
      default: "",
    },
    modelValue: {
      type: String,
      default: "",
    },
    label: {
      type: String,
      default: "",
    },
  },
  components: { Wrapper },
};
</script>

<style scoped lang="scss">
.main {
  display: flex;
  flex-direction: column;
  text-transform: capitalize;
  label {
    color: whitesmoke;
    font-size: 43px;
  }
  input {
    width: 500px;
    outline: none;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
    border-top-right-radius: 30%;
    border-bottom-right-radius: 30%;
  }
}
</style>
