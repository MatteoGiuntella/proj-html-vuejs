<script>
export default {
  data() {
    return {};
  },
  methods: {},
};
</script>

<template>
  <header>
    <div class="container">
      <nav>
        <div class="navbar-container d-flex align-items-center ">

          <div class="box-left-navbar">
            <img src="../../public/img/dark-logo.png" alt="dark-logo.png"/>
          </div>

          <div class="box-right-navbar d-flex align-items-center ">
            <nav class="navbar navbar-expand-lg navbar ">
              <div class="container-fluid">
                <button
                  class="navbar-toggler"
                  type="button"
                  data-bs-toggle="collapse"
                  data-bs-target="#navbarNavDarkDropdown"
                  aria-controls="navbarNavDarkDropdown"
                  aria-expanded="false"
                  aria-label="Toggle navigation"
                >
                  <span class="navbar-toggler-icon"></span>
                </button>
                <div
                  class="collapse navbar-collapse"
                  id="navbarNavDarkDropdown"
                >
                  <ul class="navbar-nav">
                    <li class="nav-item dropdown">
                      <button
                        class="btn dropdown-toggle"
                        data-bs-toggle="dropdown"
                        aria-expanded="false"
                      >
                        Dropdown
                      </button>
                      <ul class="dropdown-menu dropdown-menu-dark">
                        <li>
                          <a class="dropdown-item" href="#">Action</a></li>
                      </ul>
                    </li>
                  </ul>
                </div>
              </div>
            </nav>

            <div class="item-box">
              <item></item>
              <item></item>
            </div>

            <div class="box-input">
              <form class="d-flex" role="search">
                <input
                  class="form-control me-2"
                  type="search"
                  placeholder="Search"
                  aria-label="Search"
                />
                <button class="btn btn-outline-success" type="submit">
                  Search
                </button>
              </form>
            </div>
          </div>
        </div>
      </nav>
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use "../assets/scss/main" as *;
@use "../assets/scss/partials/variables.scss" as *;
header {
  height: 80px;
  width: 100%;
  background-color: $beige;
  .container{
    nav{
      .navbar-container{
        .box-left-navbar{
          width: 300px;
          height: 70px;
          .img{
            width: 100%;
            height: 100%;
            object-fit: cover;
          }
        }

      }

    }
  }
}
</style>
