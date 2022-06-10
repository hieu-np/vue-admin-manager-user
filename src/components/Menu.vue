<template>
  <nav class="navbar navbar-dark navbar-expand-lg menu-color">
    <div class="container-fluid">
      <router-link class="navbar-brand fw-bold" to="/">User Manager</router-link>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <routerLink :class="[homePage === 0 ? 'active' : '', 'nav-link fw-bold']" aria-current="page" to="/">Dashboard</routerLink>
          </li>
          <li class="nav-item">
            <routerLink :class="[homePage === 1 ? 'active' : '', 'nav-link fw-bold']" to="/add">Add User</routerLink>
          </li>
          <li class="nav-item">
            <a :class="[homePage === 2 ? 'active' : '', 'nav-link fw-bold disble']"> Detail & Edit</a>
          </li>
         
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Menu',
  computed: {
    homePage() {
      if (this.$route.path === "/") {
        return 0;
      } else if(this.$route.path === "/add"){
        return 1;
      }else{
        return 2;
      }
    },
  },
};
</script>

<style>
.menu-color{
  background-color: rgba(13,110,253, 0.4);
  /* border-bottom: solid rgba(13,110,253, 0.4) 1px; */
  /* box-shadow: 5px 5px 10px#888888; */
}
</style>