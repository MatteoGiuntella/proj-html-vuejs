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
        <div
          class="navbar-container d-flex align-items-center justify-content-between"
        >
          <div class="box-left-navbar">
            <img src="../../public/img/dark-logo.png" alt="dark-logo.png" />
          </div>

          <div class="box-right-navbar d-flex align-items-center">
            <nav class="navbar navbar-expand-lg navbar">
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
                          <a class="dropdown-item" href="#">Action</a>
                        </li>
                      </ul>
                    </li>
                  </ul>
                </div>
              </div>
            </nav>

            <div class="item-box d-flex justify-content-around">
              <span class="box-item-shop d-flex ">
                <div class="dropdown">
                  <button
                    class="btn dropdown-toggle"
                    type="button"
                    data-bs-toggle="dropdown"
                    aria-expanded="false"
                  >
                    <i class="fa-solid fa-cart-shopping fa-sm"></i>
                  </button>
                  <div class="dropdown-menu cart-box">
                    <div class="dropdown-item mb-5 text-center">
                      <i
                        class=" fa-brands fa-opencart fa-2xl"
                        style="color: #20ad96"
                      ></i>
                    </div>
                    <h5 class=" text-center mb-3 ">Your Cart is empty</h5>
                    <button class="dropdown-item my-button " type="button">
                      Browse Shop
                    </button>
                  </div>
                </div>
                <div class="dropdown">
                  <button
                    class="btn dropdown-toggle"
                    type="button"
                    data-bs-toggle="dropdown"
                    aria-expanded="false"
                  >
                    <i class="fa-regular fa-user fa-sm"></i>
                  </button>
                  <div class="dropdown-menu">
                    <div class="dropdown-item"></div>
                  </div>
                </div>
              </span>
            </div>

            <div class="box-input input-group d-flex">
              <div class="input-group flex-nowrap">
                <input
                  type="text"
                  class="form-control"
                  placeholder="search"
                  aria-describedby="addon-wrapping"
                />
                <span class="input-group-text" id="addon-wrapping">
                  <i
                    class="fa-solid fa-magnifying-glass"
                    style="color: #20ad96"
                  ></i
                ></span>
              </div>
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
  .container {
    nav {
      .navbar-container {
        padding: 10px;
        .box-left-navbar {
          width: 150px;
          img {
            width: 100%;
          }
        }
        .box-right-navbar {
          .item-box {
            .box-item-shop {
              .cart-box{
                width: 250px;
                height: 250px;
                border: 0px solid $white;
                padding: 50px;
                .my-button{
                  width: 100%;
                  background-color: $green;
                  border: 1px solid;
                  text-align: center;
                }
              }
              
            }
          }
        }
      }
    }
  }
}
</style>
