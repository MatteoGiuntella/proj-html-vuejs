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
                            
                        </div>
                    </div>
                </div>
            </div>
            
        </section>


        <!-- SECTION 3 -->
        <section class="section_3">
            <div class="container">
                
            </div>
        </section>
        <!-- SECTION 4 -->
        <section class="section_4">
            <div class="container">
                
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
