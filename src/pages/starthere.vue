<script>
import {store} from '../store.js'
export default {
  data() {
    return {
      store,



      carouselLists: [
        {
          image: '../../public/img/stock-full-hd-03-480x298.jpg',
          title:'OPEN UP A BRIGHT SKY',
          number:'01',
          subtitle:'LIFE CONSULTANCY',
          description:'Lorem, ipsum dolor sit amet consectetur adipisicing elit. Repudiandae, fugiat Lorem ipsum dolor sit amet consectetur adipisicing elit. Natus ullam recusandae ducimus nemo quibusdam vitae, eligendi reprehenderit'
        },
        {
          image: '../../public/img/stock-full-hd-04-480x298.jpg',
          title:'AWAKEN YOUR GIFTS NOW',
          number:'02',
          subtitle:'INSPIRING CURRICULUM',
          description:'Lorem, ipsum dolor sit amet consectetur adipisicing elit. Repudiandae, fugiat Lorem ipsum dolor sit amet consectetur adipisicing'
        },
        {
          image: '../../public/img/stock-full-hd-05-480x298.jpg',
          title:'WRITE YOUR OWN LIFE BOOK',
          number:'03',
          subtitle:'SKILL ADVANCEMENT',
          description:'Lorem, ipsum dolor sit amet consectetur adipisicing elit. Repudiandae, fugiat Lorem ipsum dolor sit amet consectetur adipisicing elit. Natus ullam recusandae ducimus nemo quibusdam '
        },
      ],



      footerLeftNavs: [
        {
          title: "Address",
          list: [
            '382 NE 191st St # 87394 Miami, FL 33179-3899',
            '+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)',
            'support@maxcoach.com',
          ]
        },
      ],
      footerRightNavs:[
        {
          title: "Explore",
          list: [
            'Start here',
            'Blog',
            'About us'
          ],
        },
        {
          title: "",
          list: [
            'Success story',
            'Courses',
            'Contact us'
          ],
        },
        {
          title: "Information",
          list: [
            'Membership',
            'Purchase guide',
            'Privacy policy',
            'Terms of services'
          ],
        },
      ],
    };
  },
  methods: {
  }
}
</script>

<template>
  <main class=" pt-5">
    <div class="section-array">
      <div class="container-img text-white">
        <!-- INIZIO carousel -->
        <div id="carouselExampleAutoplaying" class="carousel slide carousel-fade" data-bs-ride="carousel">
          <div class="carousel-inner">
            <div class="carousel-item active" v-for="(carouselList, i) in carouselLists" :key="i">
              <img :src="carouselList.image" :alt="carouselList.title" class="d-block w-100">
              <div class="img-filter">

              </div>
              <div class="text-container">
                <h2>
                  {{ carouselList.title }}
                </h2>
                <div>
                  <div class="subtitle-container d-flex">
                    <h5 class="me-4">
                      {{ carouselList.number }}
                    </h5>
                    <div class="me-4">
                    </div>
                    <h5 class="me-4">
                      {{ carouselList.subtitle }}
                    </h5>
                  </div>
                  <p>
                    {{ carouselList.description }}
                  </p>
                </div>
              </div>
            </div>
          </div>
          <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleAutoplaying" data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
          </button>
          <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleAutoplaying" data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
          </button>
        </div>
      </div>
      <!-- FINE carousel -->
      
    </div>
    <!-- FINE section-array -->
    

    <div class="container">
      <div class="section-steps text-center mt-5">
        <p>
          FOUR MAJOR STEPS TO SUCCESS
        </p>
        <h2 class="fw-bold mb-5">
          Best chances for expanding your success to the max
        </h2>

        <div class="section-broadening">
          
          <!-- immagine a sinistra -->
          <div class="row">
            <div class="col ">
              <div class="row">
                <div class="col-6 p-5 border-middle ">
                  <div class=" position-relative w-100 ">
                    <h3 class="fw-bold d-flex justify-content-end ">
                      BROADENING
                    </h3>
                    <div class="timeline-dot-right">
                      <div class="timeline-all-dot-right">
                      </div>
                    </div>
                  </div>
                  <div class="container-img mt-5 ">
                    <img src="../../public/img/stock-full-hd-03-480x298.jpg" alt="">
                  </div>
                </div>
                <!-- FINE col -->
                <div class="col-6 p-5  position-relative">
                  <div class="container-text text-start">
                    <h4 class="fw-bold">
                      #1 Career advancement and hobbies
                    </h4>
                    <p class="mt-4 fs-5 ">
                      Studying online gives you more flexibility. You can work and fit your work schedule around your coursework more easily; even more so if you are taking an asynchronous class: an online class where you can study and interact with your instructor and fellow classmates at your own pace.                    </p>
                  </div>
                </div>
                <!-- FINE col -->
              </div>
              <!-- FINE row -->
            </div>
            <!-- FINE col -->
          </div>
          <!-- FINE row -->

          <!-- immagine a destra -->
          <div class="row">
            <div class="col ">
              <div class="row">
                <div class="col-6 border-middle p-5 position-relative">
                  <div class="container-text text-end">
                    <h4 class="fw-bold">
                      #2 Flexible schedule & environment
                    </h4>
                    <p class="mt-4 fs-5">
                      Taking an online course also means that you don’t have to commute to class, which means less time spent on the bus and more study time sitting on your couch, the sound of a crackling fireplace in the background. You no longer have to worry about missing an important class!                    </p>
                  </div>
                </div>
                <!-- FINE col -->
                <div class="col-6 p-5 ">
                  <div class="prova-container position-relative w-100 ">
                    <h3 class="fw-bold d-flex justify-content-start ">
                      SCHEDULING
                    </h3>
                    <div class="timeline-dot-left">
                      <div class="timeline-all-dot-left">
                      </div>
                    </div>
                  </div>
                  <div class="container-img mt-5 ">
                    <img src="../../public/img/stock-full-hd-04-480x298.jpg" alt="">
                  </div>
                </div>
                <!-- FINE col -->
              </div>
              <!-- FINE row -->
            </div>
            <!-- FINE col -->
          </div>
          <!-- FINE row -->


          <!-- immagine a sinistra -->
          <div class="row">
            <div class="col ">
              <div class="row">
                <div class="col-6 p-5 border-middle ">
                  <div class="prova-container position-relative w-100 ">
                    <h3 class="fw-bold d-flex justify-content-end ">
                      SELF-DISCIPLINE
                    </h3>
                    <div class="timeline-dot-right">
                      <div class="timeline-all-dot-right">
                      </div>
                    </div>
                  </div>
                  <div class="container-img mt-5 ">
                    <img src="../../public/img/stock-full-hd-05-480x298.jpg" alt="">
                  </div>
                </div>
                <!-- FINE col -->
                <div class="col-6 p-5  position-relative">
                  <div class="container-text text-start">
                    
                    <h4 class="fw-bold">
                      #3 Self-discipline & responsibility
                    </h4>
                    <p class="mt-4 fs-5">
                      Who says that having to be more self-disciplined is a disadvantage? It is true that studying online requires more time-management skills, because you will spend a lot of time on your own without someone physically close to keep you focused on deadlines.                     </p>
                  </div>
                </div>
                <!-- FINE col -->
              </div>
              <!-- FINE row -->
            </div>
            <!-- FINE col -->
          </div>
          <!-- FINE row -->

          <!-- immagine a destra -->
          <div class="row">
            <div class="col ">
              <div class="row">
                <div class="col-6 border-middle p-5 position-relative">
                  <div class="container-text text-end">
                    <h4 class="fw-bold">
                      #4 Smart investment into future
                    </h4>
                    <p class="mt-4 fs-5">
                      Studying online means that you pay the tuition fee, possibly book supplies, an online application fee, and few other items. You don’t, however, incur the costs of housing (which can range up to $12,000 per year) and transportation, which translates to lower debts and more savings.                    </p>
                  </div>
                </div>
                <!-- FINE col -->
                <div class="col-6 p-5 ">
                  <div class="prova-container position-relative w-100 ">
                    <h3 class="fw-bold d-flex justify-content-start ">
                      INVESTMENT
                    </h3>
                    <div class="timeline-dot-left">
                      <div class="timeline-all-dot-left">
                      </div>
                    </div>
                  </div>
                  <div class="container-img mt-5 ">
                    <img src="../../public/img/stock-full-hd-06-480x298.jpg" alt="">
                  </div>
                </div>
                <!-- FINE col -->
              </div>
              <!-- FINE row -->
            </div>
            <!-- FINE col -->
          </div>
          <!-- FINE row -->
          
        </div>
        <!-- FINE section-broadening -->
      </div>
      <!-- FINE section-steps -->

    </div>
    <!-- FINE section-steps -->

    <div class="section-register">
      <div class="container text-center mt-5">
        <p>
          GET YOURSELF A 
          <b>
            MAXCOACH
          </b> 
          ID?
        </p>
        <h2 class="fw-bold mb-5">
          Take your interest and register an online class today to enjoy life fully        </h2>

        <button type="button" class="btn text-white fw-bold fs-6">
          Get started for free
        </button>
      </div>
      <!-- FINE container button-->

      <div class="section-images mt-5 d-flex flex-wrap">
        <div class="row">
          <div class="col-5 img-container">
            <img src="../../public/img/stock-full-hd-05-480x298.jpg" alt="">
            <div class="overlay text-center text-white ">
              <div class="text">
                <h3 class="fw-bold fs-1">
                  Lonnie Marks
                </h3>
                <p>
                  Tutor
                </p>
              </div>
            </div>
          </div>
          <div class="col-7 img-container">
            <img src="../../public/img/stock-full-hd-03-480x298.jpg" alt="">
            <div class="overlay text-center text-white ">
              <div class="text">
                <h3 class="fw-bold fs-1">
                  Britney Salker
                </h3>
                <p>
                  Educator
                </p>
              </div>
            </div>
          </div>
          <div class="col-8 img-container">
            <img src="../../public/img/stock-full-hd-04-480x298.jpg" alt="">
            <div class="overlay text-center text-white ">
              <div class="text">
                <h3 class="fw-bold fs-1">
                  Bronnies Wallz
                </h3>
                <p>
                  Alumnis 
                </p>
              </div>
            </div>
          </div>
          <div class="col-4 img-container">
            <img src="../../public/img/testimonial-avata-02.jpg" alt="">
            <div class="overlay text-center text-white ">
              <div class="text">
                <h3 class="fw-bold fs-1">
                  Mia Paulo
                </h3>
                <p>
                  Writer
                </p>
              </div>
            </div>
          </div>
          <div class="col-6 img-container">
            <img src="../../public/img/stock-full-hd-06-480x298.jpg" alt="">
            <div class="overlay text-center text-white ">
              <div class="text">
                <h3 class="fw-bold fs-1">
                  Lina Esthers
                </h3>
                <p>
                  Author
                </p>
              </div>
            </div>
          </div>
          <div class="col-6 img-container">
            <img src="../../public/img/stock-full-hd-05-480x298.jpg" alt="">
            <div class="overlay text-center text-white ">
              <div class="text">
                <h3 class="fw-bold fs-1">
                  Lorean McPhils
                </h3>
                <p>
                  Designer
                </p>
              </div>
            </div>
          </div>
          <div class="col-4 img-container">
            <img src="../../public/img/testimonial-avata-01.jpg" alt="">
            <div class="overlay text-center text-white ">
              <div class="text">
                <h3 class="fw-bold fs-1">
                  Anna Muray
                </h3>
                <p>
                  Writer
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>

    </div>
    <!-- FINE section-register -->

    <div class="section-accordion mt-5"> 
      <div class="container text-center">
        <p>
          SUCCEED WITH 
          <b>
            MAXCOACH
          </b>
        </p>
        <h2 class="fw-bold mb-5">
          Frequently asked questions
          
        </h2>
        <div class="row">
          <div class="col accordion-container">
            
            <!-- ACCORDION left-->
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
            <!-- FINE  accordion -->
          </div>
          <!-- FINE col -->

          <div class="col accordion-container">
            <!-- ACCORDION right-->
            <div class="accordion" id="accordionExample">
              <div class="accordion-item mb-4">
                <h2 class="accordion-header">
                  <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour" aria-expanded="true" aria-controls="collapseFour">
                    Multiple Platforms Supported for Teaching & Studying
                  </button>
                </h2>
                <div id="collapseFour" class="accordion-collapse collapse show" data-bs-parent="#accordionExample">
                  <div class="accordion-body">
                    <span class="color_dark_gray">
                      MaxCoach supports the act of teaching and learning on multiple platforms like online or offline via material downloads. We know things aren't supposed to be devoured in a short time, you can always access our knowledge base from any device.
                    </span>
                  </div>
                </div>
              </div>
              <div class="accordion-item mb-4">
                <h2 class="accordion-header">
                  <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFive" aria-expanded="false" aria-controls="collapseFive">
                    Multiple Course Participation at the Same Time
                  </button>
                </h2>
                <div id="collapseFive" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                  <div class="accordion-body">
                    Study for a number of courses at the same time is possible as long as you can afford the fee and time for completing them in the proper time. Learn at your own desired timeline and timetable. Maximum up to 5 course at a time for a learner at MaxCoach.
                  </div>
                </div>
              </div>
              <div class="accordion-item mb-4">
                <h2 class="accordion-header">
                  <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSix" aria-expanded="false" aria-controls="collapseSix">
                    Track Study Progress & Deliver Prompt Feedback
                  </button>
                </h2>
                <div id="collapseSix" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                  <div class="accordion-body">
                    It's not just a normal thing to be able to build such a solid online educational system like MaxCoach where your progress is easily tracked and feedback is properly delivered. We promise to keep improving our system for better stability and flexibility.
                  </div>
                </div>
              </div>
            </div>
            <!-- FINE  accordion -->
          </div>
        </div>
      </div>
    </div>
  </main> 

  <footer class=" mt-5 p-5">
    <div class="container">
      <div class="row">
        <div class="col-6">
          <div class="list-container" v-for="(footerLeftNav, i) in footerLeftNavs">
            <div class="fw-bold fs-5">
              {{ footerLeftNav.title }}
            </div>
            <ul>
              <li  v-for="(listOne, j) in footerLeftNav.list">
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
        <div class="col-6 d-flex ">
          <div class="list-container" v-for="(footerRightNav, i) in footerRightNavs">
            <div class="fw-bold fs-5">
              {{ footerRightNav.title }}
            </div>
            <ul>
              <li v-for="(listOne, j) in footerRightNav.list">
                <a href="#">
                  {{ listOne}}
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
          <p>
            © 2020 Maxcoach. All Rights Reserved
          </p>
        </div>
      </div>
    </div>
    <!-- FINE container -->
  </footer> 
</template>

<style lang="scss" scoped>
  @use '../assets/scss/starthere.scss';
  @use '../assets/scss/partials/variables.scss' as *;
</style>
