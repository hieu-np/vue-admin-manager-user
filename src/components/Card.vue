<template>
  <div class="row user-list p-3">
    <div class="col col-12 col-sm-12 col-md-12 col-lg-12 col-xl-10">
      <div class="card card-style">
        <div class="card-header card-header-style">Header</div>
        <div class="card-body text-dark">
          <h5 class="card-title">Dark card title</h5>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
};
</script>

<style>
.user-list {
  display: flex;
  justify-content: center;
}
.card-header-style {
  border-top: 4px solid #1d1d1d ;
  border-radius: 10px !important;
}
.card-style {
  border: 0px !important;
  border-radius: 10px !important;
  background-color: rgba(110, 166, 219, 0.5) !important;
  box-shadow: 5px 10px 30px #1d1d1d;
}
</style>