<script>
import { store } from "../store.js";
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";
import component2 from "../components/components home page/component2.vue";
import footertop from "../components/components footer top/footertop.vue";
import offcanvas  from "../components/components home page/offcanvas.vue";
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
          img: "/img/testimonial-avata-01.jpg",
          content:
            "lorem ipsum , Lorem ipsum, dolor sit amet consectetur adipisicing elit. Rem, enim quos id aperiam soluta accusantium?",
          name: "alex telles",
          role: "/Private Tutor",
        },
        {
          img: "/img/testimonial-avata-02.jpg",
          content:
            "lorem ipsum , Lorem ipsum, dolor sit amet consectetur adipisicing elit. Rem, enim quos id aperiam soluta accusantium?",
          name: "Marcus Fletcher",
          role: "/MArketing",
        },
        {
          img: "/img/testimonial-avata-03.jpg",
          content:
            "lorem ipsum , Lorem ipsum, dolor sit amet consectetur adipisicing elit. Rem, enim quos id aperiam soluta accusantium?",
          name: "Sally Coiler",
          role: "/Assistant",
        },
        {
          img: "/img/testimonial-avata-04.jpg",
          content:
            "lorem ipsum , Lorem ipsum, dolor sit amet consectetur adipisicing elit. Rem, enim quos id aperiam soluta accusantium?",
          name: "Mauro Rossi",
          role: "/Ceo",
        },
      ],
      slider: [
        {
          icon: "client-logo-colored-01.png",
        },
        {
          icon: "client-logo-colored-02.png",
        },
        {
          icon: "client-logo-colored-03.png",
        },
        {
          icon: "client-logo-colored-04.png",
        },
        {
          icon: "client-logo-colored-05.png",
        },
        {
          icon: "client-logo-colored-06.png",
        },
      ],
    };
  },
  components: {
    Swiper,
    SwiperSlide,
    component2,
    footertop,
    offcanvas
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
  <div>
    <offcanvas />
  <section class=" bg-section-1 pt-5 ">
    <div class="container pt-5 ">
      <router-link
                class="px-1 text-decoration-none text-black"
                :to="{ name: 'home' }"
              >
                Home</router-link
              >/
              <router-link
                class="px-1 text-decoration-none text-black"
                :to="{ name: 'aboutus' }"
              >
                About Us</router-link
              >
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
              v-for="(elem, i) in date" :key="i"
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
            <img :src="getImagePath('/img/' + elem.icon)" alt="" />
          </swiper-slide>
        </swiper>
      </div>
    </div>
  </div>

  <!-- section 4 -->
<section class="bg">
  <div class="container pt-5 ">
    <div class="row my-5">
        <div class="col-12 text-center ">
            <h5>MAXIMIZE YOUR POTENTIALS</h5>
        </div>
    </div>

    <div class="row my-5 ">
      <div class="col-12 text-xl-center">
        <span
          ><h1>Things we <span class="hearts">Can Help</span> you</h1></span
        >
      </div>
    </div>

    <div class="row">
       
        <div class="col-6">
            <div class="cart mb-5 pt-2">
                <div class=" mb-3 ">
                    <h2><i class="fa-regular fa-flag fa-2xl" style="color: #000000;"></i></h2>
                </div>
                <h5>Life Mentoring</h5>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam perspiciatis voluptatum delectus, quidem neque </p>
            </div>
            <div class="cart mb-5 pt-2">
                <div class=" mb-3">
                    <h2><i class="fa-solid fa-hammer fa-2xl" style="color: #000000;"></i></h2>
                </div>
                <h5>Self Development</h5>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam perspiciatis voluptatum delectus, quidem neque </p>
            </div>
            <div class="cart mb-5 pt-2">
                <div class="mb-3">
                    <h2><i class="fa-solid fa-anchor fa-2xl" style="color: #000000;"></i></h2>
                </div>
                <h5>Ask Consulantancy</h5>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam perspiciatis voluptatum delectus, quidem neque </p>
            </div>
            <div class="cart mb-5 pt-2">
                <div class="mb-3">
                    <h2><i class="fa-solid fa-display fa-2xl" style="color: #000000;"></i></h2>
                </div>
                <h5>Remote Learning</h5>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam perspiciatis voluptatum delectus, quidem neque </p>
            </div>
        </div>
        <div class="col-6">
           <div class="bg-box ps-5 pt-5">   
             <img class=" w-100 " src="../../public/img/about-us-03-image-02.png" alt="">
           </div>
        </div>

    </div>
  </div>
</section> 
  <footertop />
</div>
</template>

<style lang="scss" scoped>
@use "../assets/scss/aboutus.scss";
@use "../assets/scss/partials/variables.scss" as *;
section {
    background-color: #FCFCFC;
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
// section 4
.bg{
  background-color: rgb(240, 240, 240);
}
.bg-box{
    // background-image: url("../../public/img/home-5-image-box-01.png");
    // background-size: contain;
    // background-repeat: no-repeat;
    // background-position: center;
    height: 200px;
    width: 100%;
    img{
      max-width: 80%;
    }
}

</style>
