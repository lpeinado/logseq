<script setup>
const isMobileNavOpen = ref(false)
</script>

<template>
  <nav class="navbar">
    <div class="container">
      <div class="navbar-brand">
        <nuxt-link to="/" class="navbar-item has-text-weight-bold is-size-5">
          <div class="button">Home</div>
        </nuxt-link>
        <nuxt-link to="/dashboard" class="navbar-item has-text-weight-bold is-size-5">
          <div class="button">Dashboard</div>
        </nuxt-link>
      </div>
    </div>
  </nav>
</template>

<style>
  .navbar{
    position: sticky;
    z-index: 2;
    top: 0;
  }
  .container{
    justify-content: flex-end;
  }
</style>
