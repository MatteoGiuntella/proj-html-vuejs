<script>
import {store} from '../store.js'
export default {
    data() {
        return {
            store,
            section1:[
                {
                    url: "home-5-image-box-01.png",
                    name: "Idea Discussion",
                    description: "Get teamed up with the specialist who work and teach coding for years years at famous universities"
                },
                {
                    url: "home-5-image-box-02.png",
                    name: "Web Development",
                    description: "Learn to start building a webpage from scratch. You decide your own pace, course and speed."
                },
                {
                    url: "home-5-image-box-03.png",
                    name: "System Administration",
                    description: "Learners are encouraged to study the mechanism and structure of system administration."
                },
                {
                    url: "home-5-image-box-04.png",
                    name: "Graphic Design",
                    description: "Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness."
                },
            ],

            widgetNumber:[
                {
                    data: 1926,
                    info: "FINISHED SESSIONS"
                },
                {
                    data: 3.092 + "+",
                    info: "ENROLLED LEARNERS"
                },
                {
                    data: 200,
                    info: "ONLINE INSTRUCTORS"
                },
                {
                    data: 100 + "%",
                    info: "SATISFACTION RATE"
                },
            ],
            courses:[
                {
                    imgService: "course-02-480x298.jpg",
                    nameOwner: "Owen Christ",
                    imgOwner: "73ee246daf47502812ccefc84bf02898.jpeg",
                    service: "Personal Finance: Financial Security Thinking & Principles",
                    lessons: 2,
                    student: 299,
                    price: "Free"
                },
                {
                    imgService: "course-02-480x298.jpg",
                    nameOwner: "Blanche Fields",
                    imgOwner: "73ee246daf47502812ccefc84bf02898.jpeg",
                    service: "Learning to Write as a Professional Author",
                    lessons: 20,
                    student: 77,
                    price: "$40.00"
                },
                {
                    imgService: "stock-full-hd-03-480x298.jpg",
                    nameOwner: "Maggie Strickland",
                    imgOwner: "d0d504142acfde820eef2f11feea6253.jpeg",
                    service: "Customer-centric Info-Tech Strategies",
                    lessons: 24,
                    student: 956,
                    price: "Free"
                },
                {
                    imgService: "stock-full-hd-04-480x298.jpg",
                    nameOwner: "Maggie Strickland",
                    imgOwner: "d0d504142acfde820eef2f11feea6253.jpeg",
                    service: "Open Programming Courses for Everyone: Python",
                    lessons: 17,
                    student: 66,
                    price: "19.00"
                },
                {
                    imgService: "stock-full-hd-06-480x298.jpg",
                    nameOwner: "Blanche Fields",
                    imgOwner: "73ee246daf47502812ccefc84bf02898.jpeg",
                    service: "Academic Listening and Note-taking",
                    lessons: 14,
                    student: 68,
                    price: "$26.00"
                },
                {
                    imgService: "course-featured-image-01-480x298.jpg",
                    nameOwner: "Blanche Fields",
                    imgOwner: "73ee246daf47502812ccefc84bf02898.jpeg",
                    service: "Master jQuery in a Short Period of Time",
                    lessons: 6,
                    student: 51,
                    price: "$39.00"
                },
            ]
        };
    },
    methods: {

    }
}
</script>

<template>
    <div class="homePage_container">

        <!-- JUMBO -->
        <div class="jumbo_container">
            <div class="container">
                <div class=" row p-4 ">
                    <div class="col-6 left_jumbo_container">
                        <h2 class=" mb-4">
                            Complete Your 
                            <br> Dreams  in JavaS 
                            <br> Programming
                        </h2>
                        <p class=" mb-4">
                            Learn any coding program in distance and for a reasonable fee. You don't have to struggle alone, you've got our assistance and help.
                        </p>
                        <div>
                            <button class="btn btn-success ">
                                <i class="fa-solid fa-download"></i>
                                Download free E-book
                            </button>
                        </div>
                    </div>
                    <div class="col-6 right_jumbo_container">
                        <div class="img_jumbo_container">
                            <img src="/img/home-5-hero-image.png" alt="">
                        </div>
                    </div>
                </div>
            </div>
        </div>


        <!-- SECTION 1 -->
        <section class="section_1">
            <div class="container">
                <h6 class=" text-center ">
                    START LEARNING CODING LANGUAGES
                </h6>
                <div class=" text-center mb-5 ">
                    <span>
                        Build Your Dream 
                    </span>
                    
                    <span>
                        TODAY
                    </span>
                </div>

                <div class="row">
                    <div class="col-3" v-for="(elem, i) in section1" :key="i">
                        <div class="img-card-container">
                            <img :src="'/img/' + elem.url" alt="IMG not found">
                        </div>
                        <div class="text-center info-card-container">
                            <div class="title_card_section1">
                                {{elem.name}}
                            </div>
                            <div class="description_card_section">
                                {{elem.description}}
                            </div>
                            <div class="">
                                <a href="#">
                                    Start now 
                                    <i class="fa-solid fa-arrow-right-long"></i>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>   


        <!-- SECTION 2 -->
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
                        <div>
                            ACCORDION
                        </div>
                    </div>
                </div>
            </div>
            
        </section>


        <!-- SECTION 3 -->
        <section class="section_3">
            <div class="container">
                <div class="row little_container">
                    <div class="col-3" v-for="(elem, i) in widgetNumber" :key="i">
                        <div class="number_section_3">
                            {{ elem.data }}
                        </div>
                        <div class="info_section_3">
                            {{ elem.info }}
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- SECTION 4 -->
        <section class="section_4">
            <div class="container">
                <div class=" text-center info_section_4 mb-4">
                    <div class="text-secondary-grey">CHOOSE WHERE YOU'D LIKE TO BEGIN</div>
                    <span class="text-big-purple">Latest Featured </span>
                    <span class="text-green">Courses</span>
                </div>

                <div class="card_service_container">
                    <div class="row">
                        <div class="col-4 mb-4 d-flex" v-for="(course, i) in courses" :key="i">
                            <div class="card w-100 position-relative ">
                                <img :src="'/img/' + course.imgService"  class="card-img-top" alt="...">
                                <div class="card-body">
                                    <div class="d-flex">
                                        <div class="img_person">
                                            <img :src="'/img/' + course.imgOwner" alt="img">
                                        </div>
                                        <div class="name_card">
                                            {{course.nameOwner}}
                                        </div>
                                    </div>
                                    <p class="card-text">
                                        <strong>
                                            {{course.service}}
                                        </strong>
                                    </p>
                                    <div class="d-flex color_dark_gray">
                                        <div class=" me-3 ">
                                            <i class="fa-regular fa-file-lines"></i>
                                            Lessons 
                                        </div>
                                        <div>
                                            <i class="fa-regular fa-user"></i>
                                            {{course.student}} student
                                        </div>
                                    </div>
                                </div>
                                <div class="price_card_container">
                                    {{course.price}}
                                </div>
                            </div>
                        </div> 
                    </div>
                    <div class=" text-center ">
                        <button>
                            <a href="#">
                                View all courses 
                                <i class="fa-solid fa-arrow-right-long"></i>
                            </a>
                        </button>    
                    </div>

                </div>
            </div>
        </section>
        <!-- SECTION 5 -->
        <section class="section_5">
            <div class="container">
                
            </div>
        </section>
        <!-- SECTION 6 -->
        <section class="section_6">
            <div class="container">
                
            </div>
        </section>  
        <!-- SECTION 7 -->
        <section class="section_7">
            <div class="container">
                
            </div>
        </section>
        <!-- SECTION 8 -->
        <section class="section_8">
            <div class="container">
                
            </div>
        </section>
        <!-- SECTION 9 -->
        <section class="section_9">
            <div class="container">
                
            </div>
        </section>
    </div>
   
</template>

<style lang="scss" scoped>
@use '../assets/scss/home.scss';

</style>
