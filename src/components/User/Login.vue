<template>
  <div class="login">
    <h1>login</h1>
    <Input label="full name" type="text" placeholder="enter full name" />
    <Input label="username" type="text" placeholder="enter username" />
    <Input label="email" type="email" placeholder="enter email" />
    <Input label="gender" type="gender" placeholder="enter gender" />
    <Input label="password" type="password" placeholder="enter password" />
    <Button text="login" type="submit" class="btn btn-success"></Button>
  </div>
</template>
<script>
import Wrapper from "./../Dashboard/index.vue";
import Input from "./../Input/index.vue";
import Button from "./../Button/index.vue";
export default {
  name: "Login",
  components: { Wrapper, Input, Button },
};
</script>

<style scoped lang="scss">
.login {
  position: absolute;
  top: 20%;
  left: 36%;
  h1 {
    font-weight: 500;
  }
  .btn {
    margin-top: 1rem;
  }
}
</style>
