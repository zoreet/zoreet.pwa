<template>
  <div class="navbar">
    <router-link class="link" to="/">Tasks</router-link>
    <router-link class="link" to="/report">Reports</router-link>
    <router-link class="link" to="/settings">Settings</router-link>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.navbar {
  display: flex;
  padding-bottom: constant(safe-area-inset-bottom);
  padding-bottom: env(safe-area-inset-bottom);
  background: var(--default);
  width: 100%;
  display: flex;
  justify-content: space-between;
  z-index: 998;
  position: fixed;
  bottom: 0;
}

.editingTask .navbar {
  display: none;
}

.link {
  box-sizing: content-box;
  padding: 20px 16px;
  line-height: 20px;
  text-decoration: none;
  color: var(--default--text--strong);
  font-size: 16px;
  display: block;
}
.router-link-exact-active {
  color: var(--accent);
}
</style>
