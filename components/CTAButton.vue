<template>
  <button
    class="text-white text-lg font-bold px-8 py-4 rounded-md transition bg-gradient-to-r from-orange-600 to-orange-400 hover:from-orange-700 hover:to-yellow-600"
    @click="scrollToRegisterSection"
  >
    REGÍSTRATE YA
  </button>
</template>
  
  <script setup lang="ts">
function scrollToRegisterSection() {
  const register = document.getElementById("register");
  register?.scrollIntoView({ behavior: "smooth" });
}
</script>
  