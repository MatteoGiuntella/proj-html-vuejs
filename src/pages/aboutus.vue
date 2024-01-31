<script>
import { store } from "../store.js";
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";
import component2 from "../components/components home page/component2.vue";
export default {
  data() {
    return {
      store,
      counter: 0,
      date: [
        {
          number: "1.903",
          title: "FINISHED SESSION",
        },
        {
          number: "100%",
          title: "SATISFACTION RATE",
        },
        {
          number: "3092+",
          title: "ENROLLMENT FORMS",
        },
        {
          number: "200",
          title: "ONLINE INSTRUCTORS",
        },
      ],
      card: [
        {
          img: "../../public/img/testimonial-avata-01.jpg",
          content:
            "lorem ipsum , Lorem ipsum, dolor sit amet consectetur adipisicing elit. Rem, enim quos id aperiam soluta accusantium?",
          name: "alex telles",
          role: "/Private Tutor",
        },
        {
          img: "../../public/img/testimonial-avata-02.jpg",
          content:
            "lorem ipsum , Lorem ipsum, dolor sit amet consectetur adipisicing elit. Rem, enim quos id aperiam soluta accusantium?",
          name: "Marcus Fletcher",
          role: "/MArketing",
        },
        {
          img: "../../public/img/testimonial-avata-03.jpg",
          content:
            "lorem ipsum , Lorem ipsum, dolor sit amet consectetur adipisicing elit. Rem, enim quos id aperiam soluta accusantium?",
          name: "Sally Coiler",
          role: "/Assistant",
        },
        {
          img: "../../public/img/testimonial-avata-04.jpg",
          content:
            "lorem ipsum , Lorem ipsum, dolor sit amet consectetur adipisicing elit. Rem, enim quos id aperiam soluta accusantium?",
          name: "Mauro Rossi",
          role: "/Ceo",
        },
      ],
      slider: [
        {
          icon: "favicon-32x32.png",
        },
        {
          icon: "favicon-32x32.png",
        },
        {
          icon: "favicon-32x32.png",
        },
        {
          icon: "favicon-32x32.png",
        },
        {
          icon: "favicon-32x32.png",
        },
        {
          icon: "favicon-32x32.png",
        },
      ],
    };
  },
  components: {
    Swiper,
    SwiperSlide,
    component2
  },
  methods: {
    getImagePath: function (imgPath) {
      return new URL(imgPath, import.meta.url).href;
    },
    getCarousel () {
        setInterval(() => {
            if (this.counter < this.card.length -1) {
                this.counter++
            }
            else{
                this.counter = 0
            }
        }, 3000);
     
    },
  },
  mounted(){
    this.getCarousel()
  }
};
</script>

<template>
  <section>
    <div class="container">
      <div class="row my-5">
        <div class="col-6">
          <h5>EVERYTHING IS MAXCOACH</h5>

          <div>
            <h1>
              MAXIMIN YOUR <br />
              WITH POTENTIALS
            </h1>
            <h2>MAX COACH EDU</h2>
          </div>

          <P
            >We love to inspire and guide you through any subject,<br />
            develop new skills or upgrade your educational background.</P
          >

          <div>
            <span>Have a questions?</span
            ><span
              ><a href=""
                >Get Free Quote<i
                  class="fa-solid fa-arrow-right"
                  style="color: #20ad96"
                ></i></a
            ></span>
          </div>
        </div>
        <div class="col-6">
          <div class="row justify-content-center align-items-center flex-wrap">
            <div
              v-for="(elem, i) in date"
              class="col-6 justify-content-center align-items-end"
            >
              <h1>{{ elem.number }}</h1>
              <h5>{{ elem.title }}</h5>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- section 2 -->
  <section class="section_2">
    <div class="container">
      <component2 />
    </div>
  </section>

  <!-- section 3 -->
  <div class="container">
    <div class="row my-5 ">
      <div class="col-12 text-xl-center">
        <span
          ><h1>Why Do People <span class="hearts">*Hearts*</span> Us?</h1></span
        >
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-5 d-flex ">
        <div class="card-img d-flex justify-content-center ">
          <img class=" rounded-circle" :src="card[counter].img" alt="" />
        </div>
      </div>
      <div class="col-5 d-flex flex-column justify-content-center ">
        <p>{{ card[counter].content }}</p>
        <h4>{{ card[counter].name }}</h4>
        <h5>{{ card[counter].role }}</h5>
      </div>
    </div>
    <div class="row">
      <div class="col-12 my-5 ">
        <swiper
          :slidesPerView="5"
          :spaceBetween="30"
          :loop="true"
          
          class="mySwiper"
        >
          <swiper-slide v-for="(elem, i) in slider">
            <img :src="getImagePath('../../public/img/' + elem.icon)" alt="" />
          </swiper-slide>
        </swiper>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/scss/aboutus.scss";
@use "../assets/scss/partials/variables.scss" as *;
section {
  div {
    div {
      div {
        div {
          h1 {
            font-weight: bold;
          }
          h2 {
            color: $green;
          }
        }
        p {
        }
        div {
          span {
            a {
              text-decoration: none;
              color: $green;
              font-weight: bold;
            }
          }
        }
      }
      div {
        div {
          div {
            h1 {
              font-size: 40px;
              color: $green;
            }
          }
        }
      }
    }
  }
}
// // section 2
// .section_2 {
//   margin-top: 50px;
//   margin-bottom: 50px;
//   .text-information-container {
//     span:first-of-type,
//     span:last-of-type {
//       color: $purple;
//       font-size: 2.7em;
//       font-weight: 600;
//     }
//     span:nth-of-type(2) {
//       color: $green;
//       font-size: 2.7em;
//       font-weight: 300;
//     }
//   }
//   //accordion
//   .accordion-button:not(.collapsed) {
//     background-color: $green;
//     color: white;
//     box-shadow: none;
//   }

//   .accordion-button.collapsed::after {
//     background: url("/img/plus.svg");
//     background-size: contain;
//   }

//   .accordion-button:not(.collapsed)::after {
//     background: url("/img/minus.png");
//     background-size: contain;
//   }
// }
// .img_container_section2 {
//   display: flex;
//   justify-content: center;
//   img {
//     display: block;
//   }
// }

// section 3
.hearts{
    color: $green;
}
.swiper {
  width: 100%;
  height: 100%;
}

.swiper-slide {
  text-align: center;
  font-size: 18px;
  background: #fff;

  /* Center slide text vertically */
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
