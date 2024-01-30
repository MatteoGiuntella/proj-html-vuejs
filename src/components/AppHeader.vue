<script>
export default {
  data() {
    return {
      navbar: [
        {
          title: "Home",
          listOne: [
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
          ],
          listTwo: [
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
          ],
        },
        {
          title: "Pages",
          listOne: [
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
          ],
        },
        {
          title: "Courses",
          listOne: [
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
          ],
        },
        {
          title: "Features",
          listOne: [
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
          ],
        },
        {
          title: "Blog",
          listOne: [
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
          ],
        },
        {
          title: "Shop",
          listOne: [
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
            "lorem",
          ],
        },
      ],
    };
  },
  methods: {},
};
</script>

<template>
  <header>
    <div class="container">
      <div class="row align-items-center p-3">
        <div class="col-2">
          <img
            class="w-100"
            src="../../public/img/dark-logo.png"
            alt="dark-logo.png"
          />
        </div>

        <div class="col-6">
          
        </div>
        <div class="col-4 item-box d-flex justify-content-around">
          <span class="box-item-shop d-flex">
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
                    class="fa-brands fa-opencart fa-2xl"
                    style="color: #20ad96"
                  ></i>
                </div>
                <h5 class="text-center mb-3">Your Cart is empty</h5>
                <button class="dropdown-item my-button" type="button">
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
            </div>
          </span>

          <div class="input-group flex-nowrap">
            <input
              type="text"
              class="form-control"
              placeholder="search"
              aria-describedby="addon-wrapping"
            />
            <span class="input-group-text" id="addon-wrapping">
              <i class="fa-solid fa-magnifying-glass" style="color: #20ad96"></i
            ></span>
          </div>
        </div>
      </div>
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
    .box-left-navbar {
      width: 150px;
      img {
        width: 100%;
      }
    }
    .box-right-navbar {
      ul {
        list-style: none;
        margin: 0;
        li {
          margin-right: 10px;
        }
      }
      // .item-box {
      //   .box-item-shop {
      //     .cart-box {
      //       width: 250px;
      //       height: 250px;
      //       border: 0px solid $white;
      //       padding: 50px;

      //       .my-button {
      //         width: 100%;
      //         background-color: $green;
      //         border: 1px solid;
      //         text-align: center;

      //       }
      //     }
      //   }
      // }
    }
  }
}
</style>
