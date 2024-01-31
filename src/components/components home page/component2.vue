<script>
export default {
    data() {
        return {

        };
    },
    methods: {

    }
}
</script>

<template>
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
</template>

<style lang="scss" scoped>
@use "../../assets/scss/main.scss" as *;
@use "../../assets/scss/partials/variables.scss" as *;

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

.img_container_section2{
    display: flex;
    justify-content: center;
    img{
        display: block;
    }
}
</style>
