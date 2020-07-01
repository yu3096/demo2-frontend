<template>
  <section class="container-fluid">
    <div class="bg-stripe"></div>
    <login-component />
  </section>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'
import LoginComponent from "../components/LoginComponent";

export default {
  components: {
    AppLogo,
    LoginComponent
  }
}
</script>
<style lang="scss" scoped>
  .bg-stripe {
    position: fixed;
    height: 100vh;
    width: 600px;
    transform: skewX(20deg);
    background: linear-gradient(45deg,$primary 37%,$point-color 100%);
  }
</style>
