<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header class="lg:flex place-items-center max-h-screen pr-20 leading-8">
    <RouterLink
      class="first-of-type:border-0 inline-block px-4 py-0 border border-l border-gray-600"
      to="/"
    >
      Home
    </RouterLink>
    <RouterLink
      class="first-of-type:border-0 inline-block px-4 py-0 border border-l border-gray-600"
      to="/about"
    >
      About
    </RouterLink>
  </header>

  <RouterView />
</template>

<style scoped lang="scss">
nav a {
  &.router-link-exact-active {
    @apply text-gray-800 dark:text-white;

    &:hover {
      @apply bg-transparent;
    }
  }
}
</style>
