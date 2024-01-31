<script>
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
  methods: {},
};
</script>

<template>
  <footer>
    <div class="container button-section text-center pt-5 position-relative ">
        <img src="../../public/img/maxcoach-shape-01.png" alt="maxcoach-shape-01.png">
        <img src="../../public/img/maxcoach-shape-02.png" alt="maxcoach-shape-02.png">

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
        <div class="col text-center mt-5">
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
    background-color: $lightbeige;
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


  .button-section {
    img:first-of-type {
        position: absolute;
        top: 20%;
        left: 5%;
    }
    img:last-of-type {
        position: absolute;
        bottom: 30%;
        right: 5%;
    }

    .subtitle-section {
      span:last-child {
        color: $green;
      }
    }

    button {
      background-color: $green;
      padding: 15px 75px;
      margin-bottom: 200px;

      &:hover {
        background-color: $purple;
      }
    }
  }
  .container {
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
