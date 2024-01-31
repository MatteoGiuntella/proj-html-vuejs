<script>
import {store} from '../store.js'
export default {
  data() {
    return {
      store,
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
      ]
    };
  },
  methods: {
  }
}
</script>

<template>
  <main>
    <div class="section-array">
      <div class="container-img text-white">
        
      </div>
      
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
          PROVA SUBTITLE SECTION REGISTER
        </p>
        <h2 class="fw-bold mb-5">
          PROVA SECTION REGISTER
        </h2>

        <button type="button" class="btn text-white fw-bold fs-6">
          Large button
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

    <div class="section-accordion">
      <div class="container text-center">
        <p>
          PROVA SUBTITLE SECTION ACCORDION
        </p>
        <h2 class="fw-bold mb-5">
          PROVA SECTION ACCORDION
        </h2>

        <div class="row">
          <div class="col accordion-container">
            <div class="accordion flex-wrap" id="accordionExample">
              <div class="accordion-item">
                <h2 class="accordion-header">
                  <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
                    Accordion Item #1
                  </button>
                </h2>
                <div id="collapseOne" class="accordion-collapse collapse show" data-bs-parent="#accordionExample">
                  <div class="accordion-body">
                    <strong>This is the first item's accordion body.</strong> It is shown by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go within the <code>.accordion-body</code>, though the transition does limit overflow.
                  </div>
                </div>
              </div>
              <div class="accordion-item">
                <h2 class="accordion-header">
                  <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                    Accordion Item #2
                  </button>
                </h2>
                <div id="collapseTwo" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                  <div class="accordion-body">
                    <strong>This is the second item's accordion body.</strong> It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go within the <code>.accordion-body</code>, though the transition does limit overflow.
                  </div>
                </div>
              </div>
              <div class="accordion-item">
                <h2 class="accordion-header">
                  <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
                    Accordion Item #3
                  </button>
                </h2>
                <div id="collapseThree" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                  <div class="accordion-body">
                    <strong>This is the third item's accordion body.</strong> It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go within the <code>.accordion-body</code>, though the transition does limit overflow.
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="col accordion-container">
            <div class="accordion flex-wrap" id="accordionExample">
              <div class="accordion-item">
                <h2 class="accordion-header">
                  <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour" aria-expanded="true" aria-controls="collapseFour">
                    Accordion Item #4
                  </button>
                </h2>
                <div id="collapseFour" class="accordion-collapse collapse show" data-bs-parent="#accordionExample">
                  <div class="accordion-body">
                    <strong>This is the first item's accordion body.</strong> It is shown by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go within the <code>.accordion-body</code>, though the transition does limit overflow.
                  </div>
                </div>
              </div>
              <div class="accordion-item">
                <h2 class="accordion-header">
                  <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFive" aria-expanded="false" aria-controls="collapseFive">
                    Accordion Item #5
                  </button>
                </h2>
                <div id="collapseFive" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                  <div class="accordion-body">
                    <strong>This is the second item's accordion body.</strong> It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go within the <code>.accordion-body</code>, though the transition does limit overflow.
                  </div>
                </div>
              </div>
              <div class="accordion-item">
                <h2 class="accordion-header">
                  <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSix" aria-expanded="false" aria-controls="collapseSix">
                    Accordion Item #6
                  </button>
                </h2>
                <div id="collapseSix" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                  <div class="accordion-body">
                    <strong>This is the third item's accordion body.</strong> It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go within the <code>.accordion-body</code>, though the transition does limit overflow.
                  </div>
                </div>
              </div>
            </div>
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
                {{ listOne}}
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
