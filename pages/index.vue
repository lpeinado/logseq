<template>
  <main>
    <p v-if="!loggedIn" class="message">
        To use this app you'll need to
        <router-link to="/login">
          Login
        </router-link>
        or
        <router-link to="/register">
          Register
        </router-link>
    </p>  

  </main>
</template>
<style lang="scss" scoped>
  .message {
    color: black;
    font-size: 24px;
  }
</style>