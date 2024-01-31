<script>
import { store } from "../store.js";
export default {
  data() {
    return {
      store,
      date:[
        {
        number: "1.903",
        title: "FINISHED SESSION"
      },
      {
        number: "100%",
        title:"SATISFACTION RATE"
      },
      {
        number: "3092+",
        title:"ENROLLMENT FORMS"
      },
      {
        number: "200",
        title:"ONLINE INSTRUCTORS"
      },
    ],
      card:{
        img:"../../public/img/d0d504142acfde820eef2f11feea6253.jpeg",
        content:''
      }
    };
  },
  methods: {},
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
            WITH POTENTIALS </h1>
            <h2>MAX COACH EDU</h2>
          </div>
          
          <P
            >We love to inspire and guide you through any subject,<br> develop new
            skills or upgrade your educational background.</P
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
            <div v-for="(elem,i) in date" class="col-6 justify-content-center align-items-end ">
                <h1>{{ elem.number }}</h1>
                <h5> {{ elem.title }}</h5>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- section 2 -->
  <section class="section_2">
            <div class="container">
                <div class="row">
                    <div class=" col-6 img_container_section2">
                        <img src="/img/about-us-03-image-01.png" alt="">
                    </div>
                    <div class=" col-6 ">
                        <div class=" text-secondary ">
                            DREAM WITH 
                            <strong>MAXCOACH</strong>
                        </div>
                        <div class="text-information-container">
                            <span>Construct A </span>
                            <span>Stunning </span> <br>
                            <span>Career Perspective</span>
                        </div>
                        
                        <!-- ACCORDION -->
                        <div class="accordion" id="accordionExample">
                            <div class="accordion-item mb-4">
                                <h2 class="accordion-header">
                                <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
                                    Multiple Platforms Supported for Teaching & Studying
                                </button>
                                </h2>
                                <div id="collapseOne" class="accordion-collapse collapse show" data-bs-parent="#accordionExample">
                                <div class="accordion-body">
                                    <span class="color_dark_gray">
                                        MaxCoach supports the act of teaching and learning on multiple platforms like online or offline via material downloads. We know things aren't supposed to be devoured in a short time, you can always access our knowledge base from any device.
                                    </span>
                                </div>
                                </div>
                            </div>
                            <div class="accordion-item mb-4">
                                <h2 class="accordion-header">
                                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                                    Multiple Course Participation at the Same Time
                                </button>
                                </h2>
                                <div id="collapseTwo" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                                <div class="accordion-body">
                                    Study for a number of courses at the same time is possible as long as you can afford the fee and time for completing them in the proper time. Learn at your own desired timeline and timetable. Maximum up to 5 course at a time for a learner at MaxCoach.
                                </div>
                                </div>
                            </div>
                            <div class="accordion-item mb-4">
                                <h2 class="accordion-header">
                                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
                                    Track Study Progress & Deliver Prompt Feedback
                                </button>
                                </h2>
                                <div id="collapseThree" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                                <div class="accordion-body">
                                    It's not just a normal thing to be able to build such a solid online educational system like MaxCoach where your progress is easily tracked and feedback is properly delivered. We promise to keep improving our system for better stability and flexibility.
                                </div>
                                </div>
                            </div>
                        </div>

                        <!-- Fine accordion -->
                    </div>
                </div>
            </div>
            
        </section>

    <!-- section 3 -->
    <div class="container">
        <div class="row">
            <div class="col-12 text-xl-center ">
                <span><h1>Why Do People <span>*Hearts*</span> Us?</h1></span>
            </div>
        </div>
        <div class="row justify-content-center align-items-center ">
            <div class="col-4">
                <div class="card-img">
                    <img src="../../public/img/d0d504142acfde820eef2f11feea6253.jpeg" alt="d0d504142acfde820eef2f11feea6253">
                </div>
            </div>
            <div class="col-8">
                <p></p>
                <h4></h4>
                <h5></h5>
            </div>

        </div>
        <div class="row">
            <div class="col-2">
                <div class="img-box">
                    <img src="" alt="">
                </div>
            </div>
        </div>

    </div>


</template>

<style lang="scss" scoped>
@use "../assets/scss/aboutus.scss";
@use "../assets/scss/partials/variables.scss" as *;
section{
    div{
        div{
            div{
                div{
                    h1{
                        font-weight: bold;
                    }
                    h2{
                        color: $green;
                    }
                }
                p{
                    
                }
                div{
                    span{
                        a{
                            text-decoration: none;
                            color: $green;
                            font-weight: bold;
                        }
                    }
                }
            }
            div{
                div{
                    div{
                        h1{
                            font-size: 40px;
                            color: $green;
                        }
                    }
                }
            }
        }
    }
}
// section 2
.section_2{
    margin-top: 50px;
    margin-bottom: 50px;
    .text-information-container{
        span:first-of-type, span:last-of-type{
            color: $purple;
            font-size: 2.7em;
            font-weight: 600;
        }
        span:nth-of-type(2) {
            color: $green;
            font-size: 2.7em;
            font-weight: 300;
        }
    }
    //accordion
    .accordion-button:not(.collapsed){
        background-color: $green;
        color: white;
        box-shadow: none;
    }

    .accordion-button.collapsed::after {
        background: url("/img/plus.svg");
        background-size: contain;
      }
      
      .accordion-button:not(.collapsed)::after {
        background: url("/img/minus.png");
        background-size: contain;
      }
}
.img_container_section2{
    display: flex;
    justify-content: center;
    img{
        display: block;
    }
}

// section 3
</style>
