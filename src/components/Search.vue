<template>
  <div class="search" id="search-component">
    <i class="icofont-search-2"></i>
    <input
      type="text"
      class="searchbox"
      placeholder="Search User"
      aria-label="Username"
      id="search-box"
    />
  </div>
</template>

<script>
export default {
  name: "Search",
};
</script>

<style>
.search .icofont-search-2 {
  position: absolute;
  top: 20px;
  left: 16px;
}
.search{
    position: relative;
}
.searchbox {

  height: 40px;
  background-color: rgba(255, 255, 255, 0.5);
  border: 0px;
  border-radius: 10px;
  outline: none;
  padding-left: 10px;
}
@media only screen and (min-width: 740px) {
  .searchbox {
    width: 500px;
    margin: 0px 10px 0px 10px;
  }
}

@media only screen and (max-width: 780px) and (min-width: 550px) {
  .searchbox {
    width: 300px;
    margin: 0px 10px 0px 10px;
  }
}

@media only screen and (max-width: 550px) and (min-width: 450px) {
  .searchbox {
    width: 200px;
    margin: 0px 10px 0px 10px;
  }
}

@media only screen and (max-width: 450px) {
  .searchbox {
    width: 150px;
    margin: 0px 10px 0px 10px;
  }
}
</style>