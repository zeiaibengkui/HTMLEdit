<script setup lang="ts">
import { ref } from 'vue'
import InnerDoc from './components/InnerDoc.vue'
</script>

<template>
  <nav id="nav-bar" class="navbar navbar-expand-sm">
    <span class="navbar-brand">HTMLEdit</span>

    <div class="navbar-nav">
      <button
        class="nav-link nav-item"
        type="button"
        data-bs-toggle="offcanvas"
        data-bs-target="#file"
        aria-controls="file"
      >
        File
      </button>
      <span class="nav-item dropdown">
        <a
          class="nav-link dropdown-toggle"
          href="javascript:void(0)"
          role="button"
          data-bs-toggle="dropdown"
          aria-expanded="false"
        >
          View
        </a>
        <ul class="dropdown-menu fade">
          <li><a class="dropdown-item" href="#">Zoom +</a></li>
          <li><a class="dropdown-item" href="#">Zoom -</a></li>
          <li><hr class="dropdown-divider" /></li>
          <li><a class="dropdown-item" href="#">Dark Mode</a></li>
        </ul>
      </span>
    </div>
  </nav>

  <InnerDoc />
</template>

<style scoped lang="scss">
#nav-bar {
  width: 100%;
  background-color: white;
  backdrop-filter: blur(5px);
  box-shadow: rgba(0, 0, 0, 0.2) 0 0 3px 3px;
  --bs-navbar-padding-x: 1rem;

  .dropdown-menu {
    --bs-dropdown-spacer: calc(var(--bs-navbar-padding-y) * 2);
  }
}
</style>
