<template>
  <div class="row user-list p-3">
    <div class="col col-12 col-sm-12 col-md-12 col-lg-12 col-xl-10">
      <div class="card card-style">
        <div class="card-header card-header-style user-list-title">
          <h4 class="text-primary m-0">User Lists</h4>
          <search></search>
          <router-link to="/add" class="btn btn-primary">Add User</router-link>
        </div>
        <div class="card-body text-dark">
              <router-view></router-view>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Search from './Search.vue';
export default {
  name: "Card",
  components: {
    Search
  }
};
</script>

<style>
.user-list {
  display: flex;
  justify-content: center;
}
.user-list-title {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.card-header-style {
  border-top: 4px solid #0d6efd ;
  border-radius: 10px !important;
}
.card-style {
  border: 0px !important;
  border-radius: 10px !important;
  background-color: rgba(255, 255, 255, 0.2) !important;
  box-shadow: 5px 10px 30px #1d1d1d;
}

</style>