<script>
// import footertop from "../components/components footer top/footertop.vue";

export default {
  data() {
    return {
      footerLeftNavs: [
        {
          title: "Address",
          list: [
            "382 NE 191st St # 87394 Miami, FL 33179-3899",
            "+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)",
            "support@maxcoach.com",
          ],
        },
      ],
      footerRightNavs: [
        {
          title: "Explore",
          list: ["Start here", "Blog", "About us"],
        },
        {
          title: "",
          list: ["Success story", "Courses", "Contact us"],
        },
        {
          title: "Information",
          list: [
            "Membership",
            "Purchase guide",
            "Privacy policy",
            "Terms of services",
          ],
        },
      ],
    };
  },
  components: {
    // footertop,
  },
  methods: {},
};
</script>

<template>
  <footer>
    <div class="container">
      <div class="row">
        <div class="col-6">
          <div
            class="list-container"
            v-for="(footerLeftNav, i) in footerLeftNavs"
          >
            <div class="fw-bold fs-5">
              {{ footerLeftNav.title }}
            </div>
            <ul>
              <li v-for="(listOne, j) in footerLeftNav.list">
                {{ listOne }}
              </li>
            </ul>
          </div>
          <!-- FINE list-container -->

          <div class="social-container">
            <ul>
              <li>
                <a href="#">
                  <i class="link-icon fab fa-facebook-square"></i>
                </a>
              </li>
              <li>
                <a href="#">
                  <i class="link-icon fab fa-twitter"></i>
                </a>
              </li>
              <li>
                <a href="#">
                  <i class="link-icon fab fa-instagram"></i>
                </a>
              </li>
              <li>
                <a href="#">
                  <i class="link-icon fab fa-linkedin"></i>
                </a>
              </li>
            </ul>
          </div>
        </div>
        <!-- FINE col -->
        <div class="col-6 d-flex">
          <div
            class="list-container"
            v-for="(footerRightNav, i) in footerRightNavs"
          >
            <div class="fw-bold fs-5">
              {{ footerRightNav.title }}
            </div>
            <ul>
              <li v-for="(listOne, j) in footerRightNav.list">
                <a href="#">
                  {{ listOne }}
                </a>
              </li>
            </ul>
          </div>
          <!-- FINE list-container -->
        </div>
        <!-- FINE col -->
      </div>
      <!-- FINE row -->
      <div class="row">
        <div class="col text-center mt-3 mb-2">
          <p>© 2020 Maxcoach. All Rights Reserved</p>
        </div>
      </div>
    </div>
    <!-- FINE container -->
  </footer>
</template>

<style lang="scss" scoped>
@use "../assets/scss/main" as *;
@use "../assets/scss/partials/variables.scss" as *;

footer {
  background-color: rgb(240, 240, 240);
  ul,
  ul li,
  ul li a {
    margin: 0;
    padding: 0;
    margin-top: 10px;
    list-style-type: none;
    text-decoration: none;
    color: $darkgray;
  }
  li > a {
    &:hover {
      color: $green;
    }
  }
  .container {
    padding-top: 100px;
    .row {
      .col-6:first-child {
        .social-container {
          margin-top: 40px;
          ul {
            display: flex;
            li {
              margin-right: 40px;
              > * {
                font-size: 25px;
                &:hover {
                  color: $green;
                }
              }
            }
          }
        }
      }

      .col-6:last-child {
        .list-container {
          margin-right: 100px;
          &:nth-child(2) {
            margin-top: 31px;
          }
        }
      }

      &:last-child {
        color: #ababab;
        margin-top: 50px;
      }
    }
  }
}
</style>
