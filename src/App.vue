<template>
  <div class="app">
    <Menu></Menu>
    <Card></Card>
    <router-link to="/">Home</router-link>
    <router-link to="/detail">Detail</router-link>
    <router-link to="/add">Add</router-link>
    <router-view></router-view>
  </div>
</template>

<script>
import Menu from "./components/Menu.vue";
import Card from "./components/Card.vue";
export default {
  name: "App",
  components: {
    Menu,
    Card
},
};
</script>

<style>
html{
  height: 100%;
}
body{
  background-image: url(./assets/lake.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size:cover;
  height: 100%;
}
</style>
