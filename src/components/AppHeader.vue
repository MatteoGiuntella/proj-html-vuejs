<script>
export default {
  data() {
    return {
      homelist:[
        {
          list1:[
          "MaxCoach Education",
          "Course Portal",
          "Distant Learning",
          "Multimedia Pedagogy",
          "Modern Schooling",
          "Remote Training",
          "Health Coaching",
          "Gym Coaching",
          "Business",
          "Artist"
          ],
          list2:[
          "Kitchen Coach",
          "Motivation",
          "Dancing",
          "Guitar",
          "Yoga",
          "Photography",
          "Personal Finance",
          "Sales Coaching",
          "Mental Therapy"
          ]
        }
      ],
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
  methods: {},
};
</script>

<template>
  <header class="position-fixed">
    <div class="container position-relative">
      <div class="row align-items-center p-3">
        <div class="col-2">
          <img class="w-100" src="/img/dark-logo.png" alt="dark-logo.png" />
        </div>

        <div class="col-6 d-flex justify-content-end">
          <div class="dropdown">
            <a
              class="btn dropdown-toggle border-0 "
              href="#"
              role="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
            >
              <router-link
                class="px-1 text-decoration-none text-black cl-hov"
                :to="{ name: 'home' }"
              >
                Home</router-link
              >
            </a>

            <ul class="dropdown-menu">
              <li>
                <div class="d-flex">
                  <div class="">
                    <ul class="list-unstyled">
                      <li class="d-flex flex-column ">
                        <a class="p-2 text-decoration-none text-black cl-hov" v-for="(elem,i) in homelist[0].list1">{{ elem }} </a>
                      </li>
                      
                    </ul>
                  </div>
                  <div class="mx-2 ">
                    <ul class="list-unstyled">
                      <li class="d-flex flex-column ">
                        <a class="p-2 text-decoration-none text-black cl-hov" v-for="(elem,i) in homelist[0].list2"> {{ elem }} </a>
                      </li>
                      
                    </ul>
                  </div>
                  <div class="p-2">
                    <img src="/img/homepages-mega-menu-image-alt.jpg" alt="" />
                  </div>
                </div>
              </li>
            </ul>
          </div>
          <div
            class="dropdown d-flex justify-content-end"
            v-for="(elem, i) in navbar"
          >
            <a
              class="btn dropdown-toggle border-0 cl-hov"
              href="#"
              role="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
            >
              {{ elem.title }}
            </a>

            <div>
              <div>
                <div>
                  <ul class="dropdown-menu">
                    <li v-for="(elem, j) in navbar[i].list">
                      <a
                        v-if="
                          navbar[i].list[j] != 'Start-here' &&
                          navbar[i].list[j] != 'About-us-03'
                        "
                        class="dropdown-item text-black cl-hov"
                        href=""
                      >
                        {{ elem }}
                      </a>
                      <router-link
                        class="px-3 text-decoration-none text-black cl-hov"
                        v-else-if="navbar[i].list[j] == 'Start-here'"
                        :to="{ name: 'aboutus' }"
                      >
                        Aboutus</router-link
                      >
                      <router-link
                        class="px-3 text-decoration-none text-black cl-hov"
                        v-else-if="navbar[i].list[j] == 'About-us-03'"
                        :to="{ name: 'starthere' }"
                      >
                        Start here</router-link
                      >
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-4 item-box d-flex justify-content-around">
          <span class="box-item-shop d-flex">
            <div class="dropdown">
              <button
                class="btn dropdown-toggle position-relative "
                type="button"
                data-bs-toggle="dropdown"
                aria-expanded="false"
              >
                <i class="fa-solid fa-cart-shopping fa-sm cl-hov"></i>
                <div class="number-item">0</div>
              </button>
              <div class="dropdown-menu cart-box w-100">
                <div class="dropdown-item mb-5 text-center">
                  <i
                    class="fa-solid fa-cart-shopping fa-2xl"
                    style="color: #20ad96"
                  ></i>
                </div>
                <h5 class="text-center mb-3">Your Cart is empty</h5>
                <button class="dropdown-item my-button w-100 bg-success text-center" type="button">
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
                <i class="fa-regular fa-user fa-sm cl-hov"></i>
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
  width: 100%;
  background-color: rgba(245, 241, 237, 0.9);
  z-index: 5;
  .container {
 
    
    .box-left-navbar {
      width: 150px;
      img {
        width: 100%;
      }
    }
    }
    .number-item{
      // height: 10px;
      width: 10px;
      border-radius: 10px;
      color: white;
      font-size: 10px;
      position: absolute;
      top:0%;
      right: 35%;
      background-color: $green;
    }
    .cl-hov:hover{
      color: $green !important;
    }
    .my-button:hover{
      color: $white;
      background-color: #3F3A64 !important;
    }
  } 
</style>
