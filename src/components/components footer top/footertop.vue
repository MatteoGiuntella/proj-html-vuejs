<script>
export default {
  data() {
    return {};
  },
  methods: {},
};
</script>

<template>
  <footer class="footer-top">
    <div class="container button-section text-center pt-5 position-relative">
      <img
        src="../../../public/img/maxcoach-shape-01.png"
        alt="maxcoach-shape-01.png"
      />
      <img
        src="../../../public/img/maxcoach-shape-02.png"
        alt="maxcoach-shape-02.png"
      />

      <div class="subtitle-section">
        <span class="fs-4 fw-bold"> Start today for getting </span>
        <span class="fs-4"> Online Certification </span>
      </div>
      <h2 class="fw-bold mb-5">
        You can be your own guiding star with our help!
      </h2>

      <button type="button" class="btn text-white fw-bold fs-6">
        Get started for free
      </button>
    </div>
    <!-- FINE container button-->
  </footer>
</template>

<style lang="scss" scoped>
@use "../../assets/scss/main.scss" as *;
@use "../../assets/scss/partials/variables.scss" as *;

@keyframes line-left {
  0%   {left:5%; top:30%;}
  50%  {left:5%; top:60%;}
  100%  {left:5%; top:30%;}
}
@keyframes circle-right {
  0%   {right:5%; bottom:10%;}
  50%  {right:5%; bottom:60%;}
  100%  {right:5%; bottom:10%;}
}

.footer-top:hover img:first-of-type{
  animation-name: line-left;
  animation-duration: 2s;
  // position: relative;
}
.footer-top:hover img:last-of-type{
  animation-name: circle-right;
  animation-duration: 2s;
  // position: relative;
}

.footer-top {
  background-color: rgb(240, 240, 240);
}
.button-section {
  padding-bottom: 50px;
  img:first-of-type {
    position: absolute;
    top: 30%;
    left: 5%;
  }
  img:last-of-type {
    position: absolute;
    bottom: 10%;
    right: 5%;
  }

  img {
    transition: width 2s, height 2s, transform 2s;
  }

  .subtitle-section {
    span:last-child {
      color: $green;
    }
  }

  button {
    background-color: $green;
    padding: 15px 75px;
    

    &:hover {
      background-color: $purple;
    }
  }
}

.button-section:hover img {
  transform: rotate(360deg);
}
</style>
