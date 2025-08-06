<template>
  <div class="app-wrapper">
    <!-- Header -->
    <header class="app-header">
      <div class="container">
        <RouterLink to="/" class="logo">MySite</RouterLink>
        <nav class="nav-links">
          <RouterLink to="/">Home</RouterLink>
          <RouterLink to="/about">About</RouterLink>
          <RouterLink to="/projects">Projects</RouterLink>
          <RouterLink to="/contact">Contact</RouterLink>
        </nav>
      </div>
    </header>

    <!-- Main -->
    <main class="app-main">
      <RouterView />
    </main>

    <!-- Footer -->
    <footer class="app-footer">
      <div class="container">
        <p>© 2025 MySite. Designed by Sukhpreet.</p>
      </div>
    </footer>

    <!-- Scroll to Top -->
    <button v-show="showScroll" @click="scrollToTop" class="scroll-top" aria-label="Scroll to top">
      ↑
    </button>
  </div>
</template>

<script setup>
import { ref, onMounted, onBeforeUnmount } from 'vue'

const showScroll = ref(false)

function onScroll() {
  showScroll.value = window.scrollY > 200
}

function scrollToTop() {
  window.scrollTo({ top: 0, behavior: 'smooth' })
}

onMounted(() => window.addEventListener('scroll', onScroll))
onBeforeUnmount(() => window.removeEventListener('scroll', onScroll))
</script>

<style scoped>
/* Styles from your original message, unchanged for now */
.app-wrapper {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background-color: #fafafa;
  color: #333;
}

.app-header {
  background-color: #005f56;
  padding: 1rem 0;
  color: white;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

.container {
  max-width: 1100px;
  margin: 0 auto;
  padding: 0 1.5rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}

.logo {
  font-weight: 700;
  font-size: 1.8rem;
  color: white;
  text-decoration: none;
}

.nav-links a {
  margin-left: 1.5rem;
  color: white;
  text-decoration: none;
  font-weight: 600;
  font-size: 1rem;
  transition: color 0.3s ease;
}

.nav-links a:hover {
  color: #00bfa5;
}

.app-main {
  flex: 1;
  max-width: 1100px;
  margin: 2rem auto;
  padding: 1rem;
  background: white;
  border-radius: 8px;
  box-shadow: 0 6px 15px rgba(0,0,0,0.05);
}

.app-footer {
  background-color: #004d40;
  color: #ccc;
  text-align: center;
  padding: 1.5rem 0;
  font-size: 0.9rem;
}

.scroll-top {
  position: fixed;
  bottom: 25px;
  right: 25px;
  background-color: #005f56;
  color: white;
  border: none;
  border-radius: 50%;
  width: 45px;
  height: 45px;
  font-size: 22px;
  cursor: pointer;
  box-shadow: 0 4px 12px rgba(0,0,0,0.25);
  transition: background-color 0.3s ease;
  z-index: 1000;
}

.scroll-top:hover {
  background-color: #00bfa5;
}

@media (max-width: 768px) {
  .container {
    flex-direction: column;
    gap: 1rem;
  }
  .nav-links {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
  }
  .nav-links a {
    margin: 0 0.75rem;
  }
  .app-main {
    margin: 1rem;
  }
}
</style>
