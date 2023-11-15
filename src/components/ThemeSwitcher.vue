<script setup>
function setTheme(theme) {
  document.documentElement.setAttribute('data-bs-theme', theme)
}
</script>
<template>
  <div class="dropdown">
    <button
      class="btn dropdown-toggle"
      type="button"
      id="themeDropdown"
      data-bs-toggle="dropdown"
      aria-expanded="false"
    >
      Change Theme
    </button>
    <ul class="dropdown-menu" aria-labelledby="themeDropdown">
      <li>
        <a class="dropdown-item" href="#" @click="setTheme('light')">Light Theme</a>
      </li>
      <li>
        <a class="dropdown-item" href="#" @click="setTheme('dark')">Dark Theme</a>
      </li>
    </ul>
  </div>
</template>
