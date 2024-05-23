<template>
  <div>
    <div class="mickey-icon" @click="toggleNavbar">
      <!-- Mickey Mouse icon (can be an image or an icon library element) -->
      <img src="../assets/CROSS.png" alt="Menu Icon" />
    </div>
    <div :class="['navbar', { open: isOpen }]">
      <div class="close-icon" @click="toggleNavbar">X</div>
      <nuxt-link class="herf" to="/" exact>Home</nuxt-link>
      <nuxt-link class="herf" to="/good-movies">Good Movies</nuxt-link>
      <nuxt-link class="herf" to="/bad-movies">Bad Movies</nuxt-link>
      <nuxt-link class="herf" to="/secrets">Secrets</nuxt-link>
      <nuxt-link class="herf" to="/author">Author</nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    toggleNavbar() {
      this.isOpen = !this.isOpen;
    },
  },
};
</script>

<style scoped>
.mickey-icon {
  cursor: pointer;
  display: none; /* Hide by default, will show on small screens */
  position: fixed;
  top: 10px;
  right: 10px;
  z-index: 200;
  width: 60px;
  height: 60px;
}
.herf {
  margin-left: 10px;
  margin-right: 10px;
  text-decoration: underline;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
}

.close-icon {
  position: absolute;
  top: 10px;
  right: 10px;
  cursor: pointer;
  z-index: 201;
  font-size: 24px;
}

.navbar {
  position: fixed;
  left: -100%; /* Start off-screen */
  top: 0;
  width: 250px;
  height: 100vh;
  background-color: white;
  box-shadow: 2px 0 5px rgba(0, 0, 0, 0.5);
  display: flex;
  flex-direction: column;
  align-items: start;
  padding: 20px;
  transition: left 0.3s ease;
}

.navbar.open {
  left: 0; /* Slide in */
}

.nuxt-link {
  padding: 10px;
  margin: 5px 0;
  display: block;
  color: black;
  text-decoration: none;
}

@media (min-width: 768px) {
  .mickey-icon {
    display: none; /* Hide Mickey icon on larger screens */
  }
  .close-icon {
    display: none;
  }
  .navbar {
    position: static;
    width: auto;
    height: auto;
    display: flex;
    justify-content: center; /* Horizontal center */
    left: 0; /* Reset the left position */
    box-shadow: none;
    flex-direction: row;
    z-index: 100;
  }
}

@media (max-width: 767px) {
  .mickey-icon {
    display: block; /* Show Mickey icon on smaller screens */
  }
  .navbar {
    position: fixed;
    left: -100%; /* Start off-screen */
    top: 0;
    width: 250px;
    height: 100vh;
    background-color: white;
    box-shadow: 2px 0 5px rgba(0, 0, 0, 0.5);
    display: flex;
    flex-direction: column;
    align-items: start;
    padding: 20px;
    transition: left 0.3s ease;
    z-index: 100;
  }
}
</style>
