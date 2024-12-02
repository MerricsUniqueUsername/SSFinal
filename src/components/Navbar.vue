<template>
  <div class="navbar">
    <div class="nav-container">
      <!-- Logo -->
      <div class="logo" style="display: flex; justify-content: center;">
        <svg xmlns="http://www.w3.org/2000/svg" width="28" height="28" fill="currentColor" class="bi bi-lightning-charge" viewBox="0 0 16 16">
          <path d="M11.251.068a.5.5 0 0 1 .227.58L9.677 6.5H13a.5.5 0 0 1 .364.843l-8 8.5a.5.5 0 0 1-.842-.49L6.323 9.5H3a.5.5 0 0 1-.364-.843l8-8.5a.5.5 0 0 1 .615-.09z"/>
        </svg>
        Final
      </div>

      <!-- Desktop Navigation -->
      <div class="desktop-nav">
        <div class="navElement" v-for="item in menuItems" :key="item.label">
          <a :href="item.path">{{ item.label }}</a>
        </div>
      </div>

      <!-- Mobile Menu Toggle -->
      <div class="mobile-menu-toggle" @click="toggleMenu">
        <svg v-if="!isMenuOpen" xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-list" viewBox="0 0 16 16">
          <path fill-rule="evenodd" d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5"/>
        </svg>
        <svg v-else xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-x" viewBox="0 0 16 16">
          <path d="M4.646 4.646a.5.5 0 0 1 .708 0L8 7.293l2.646-2.647a.5.5 0 0 1 .708.708L8.707 8l2.647 2.646a.5.5 0 0 1-.708.708L8 8.707l-2.646 2.647a.5.5 0 0 1-.708-.708L7.293 8 4.646 5.354a.5.5 0 0 1 0-.708"/>
        </svg>
      </div>

      <!-- Mobile Menu -->
      <div v-if="isMenuOpen" class="mobile-menu">
        <div v-for="item in menuItems" :key="item.label" class="mobile-nav-item">
          <a :href="item.path" @click="toggleMenu">{{ item.label }}</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
  data() {
    return {
      isMenuOpen: false,
      menuItems: [
        { label: 'Home', path: '/' },
        { label: 'Map', path: '/' },
        { label: 'FAQ', path: '/' },
        { label: 'Sources', path: '/' },
      ]
    }
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen
    }
  }
}
</script>

<style scoped>
.navbar {
  position: fixed;
  width: 100vw;
  height: 80px;
  border-bottom: 1px solid rgb(29, 29, 29);
  color: white;
  background-color: black;
  z-index: 50;
}

.nav-container {
  height: 100%;
  width: 100%;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 15px;
}

.logo {
  font-size: 24px;
  font-weight: 700;
  margin-left: 50px;
}

.desktop-nav {
  display: none;
  margin-right: 50px;
}

a {
  text-decoration: none;
  color: rgba(255, 255, 255, 0.745);
  transition: 0.3s ease;
  padding: 3px 8px;
  border-radius: 50px;
  font-weight: 300;
}

a:hover {
  color: white;
  background-color: rgba(236, 236, 236, 0.303);
}

.mobile-menu-toggle {
  cursor: pointer;
  margin-right: 50px;
}

.mobile-menu {
  position: absolute;
  top: 80px;
  left: 0;
  width: 100%;
  background-color: rgba(0, 0, 0, 0.95);
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px 0;
}

.mobile-nav-item {
  margin: 10px 0;
}

.mobile-nav-item a {
  font-size: 1.2rem;
}

/* Desktop Styles */
@media (min-width: 768px) {
  .mobile-menu-toggle {
    display: none;
  }

  .desktop-nav {
    display: flex;
    align-items: center;
  }

  .navElement {
    margin-right: 20px;
  }

  .mobile-menu {
    display: none;
  }
}
</style>