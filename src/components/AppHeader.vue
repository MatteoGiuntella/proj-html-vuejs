<script>
export default {
  data() {
    return {
      navbar: [
        {
          title: "Pages",
          list: [
            "Start-here",
            "Succes story",
            "About me",
            "About-us-01",
            "About-us-02",
            "About-us-03",
            "Contact me",
            "Contact us",
            "Paurchause Guide",
            "Privacy Policy",
            "Terms of Service",
          ],
        },
        {
          title: "Courses",
          list: [
            "Courses Grid 01",
            "Courses Grid 02",
            "Courses Grid 03",
            "Membership Levels",
            "Become a Teacher",
            "Profile",
            "Checkout",
            "Single Layout",
          ],
        },
        {
          title: "Features",
          list: ["Events", "Zoom meetings"],
        },
        {
          title: "Blog",
          list: ["Blog Grid", "Blog Masonry", "Blog Classic", "Blog List"],
        },
        {
          title: "Shop",
          list: [
            "Shop left sidebar",
            "Shop right sidebar",
            "Cart",
            "Whishlist",
            "Single Product",
          ],
        },
      ],
    };
  },
  methods: {}
};
</script>

<template>
  <header>
    <router-link :to="{ name: 'aboutus' }"> aboutus</router-link>
    <div class="container position-relative">
      <div class="row align-items-center p-3">
        <div class="col-2">
          <img
            class="w-100"
            src="/img/dark-logo.png"
            alt="dark-logo.png"
          />
        </div>

        <div class="col-6 d-flex justify-content-end ">
          <div class=" d-flex position-relative ciao">
            <a  class="btn dropdown-toggle my-drop ">
              <router-link :to="{ name: 'home' }"> Home</router-link>
            </a>
          </div>
          <div
            class="dropdown d-flex justify-content-end"
            v-for="(elem, i) in navbar"
          >
            <a
              class="btn dropdown-toggle"
              href="#"
              role="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
            >
              {{ elem.title }}
            </a>

            <ul class="dropdown-menu">
              <li v-for="(elem, j) in navbar[i].list">
                <a v-if="(navbar[i].list[j] != 'Start-here') && (navbar[i].list[j] != 'About-us-03')" class="dropdown-item" href="">
                  {{ elem }}
                </a>
                <router-link v-else-if="(navbar[i].list[j] == 'Start-here')" :to="{ name: 'aboutus' }"> Aboutus</router-link>
                <router-link v-else-if="(navbar[i].list[j] == 'About-us-03')" :to="{ name: 'starthere' }"> Start here</router-link>
              </li>
            </ul>
          </div>
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
      <div class="hover-container">
        <div class="d-flex justify-content-between "> 
          <div class="d-flex">
            <ul>
              <li>Lorem Ipsum</li>
              <li>Lorem Ipsum</li>
              <li>Lorem Ipsum</li>
              <li>Lorem Ipsum</li>
              <li>Lorem Ipsum</li>
              <li>Lorem Ipsum</li>
              <li>Lorem Ipsum</li>
              <li>Lorem Ipsum</li>
            </ul>
            <ul>
              <li>Lorem Ipsum</li>
              <li>Lorem Ipsum</li>
              <li>Lorem Ipsum</li>
              <li>Lorem Ipsum</li>
              <li>Lorem Ipsum</li>
              <li>Lorem Ipsum</li>
              <li>Lorem Ipsum</li>
              <li>Lorem Ipsum</li>
            </ul>
          </div>
          <div class="mx-3">
            <img
              src="/img/homepages-mega-menu-image-alt.jpg"
              alt=""
            />
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
  width: 100%;
  background-color: $beige;
  .container {
    position: relative;
    .hover-container {
      background-color: $white;
      width: 90%;
      position: absolute;
      left: 100px;
      bottom: -280px;
      z-index: 1;
      display: none;
      ul {
        list-style: none;
        margin: 0;
        li {
          margin: 10px;
        }
      }
    }
    .ciao:active .hover-container {
        display: block;
      }

    .box-left-navbar {
      width: 150px;
      img {
        width: 100%;
      }
    }
  }
  
}
</style>
