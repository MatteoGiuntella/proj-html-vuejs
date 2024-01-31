<script>
export default {
    data() {
        return {
            previews: [
                "home-01-preview.jpg",
                "home-02-preview.jpg",
                "home-03-preview.jpg",
                "home-04-preview.jpg",
                "home-05-preview.jpg",
                "home-06-preview.jpg",
               
            ]
        };
    },
    methods: {

    }
}
</script>

<template>
    <div>
        <button class="btn btn-primary button_offacnvas text-black bg-white  border-0 " type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasRight" aria-controls="offcanvasRight">
            <div>
                <i class="fa-solid fa-ruler-combined"></i>
            </div>
            <div>
                <i class="fa-solid fa-life-ring"></i>
            </div>
            <div>
                <i class="fa-solid fa-book"></i>
            </div>
            <div>
                <i class="fa-solid fa-cart-shopping"></i>
            </div>
        </button>

        <div class="offcanvas offcanvas-end" tabindex="-1" id="offcanvasRight" aria-labelledby="offcanvasRightLabel">
            <div class="offcanvas-header p-4 ">
                <h5 class="offcanvas-title text-center " id="offcanvasRightLabel">MAXCOACH ONLINE LEARNING AND EDUCATION WORDPRESS THEME</h5>
                <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
            </div>

            <div class="offcanvas-body p-4">
                <div class="text-center">
                    <button class="btn btn-success button_shop">
                        <i class="fa-solid fa-cart-shopping"></i>
                        Buy Now
                    </button>
                    <div class="row">
                        <div class="col-6 p-1 mt-4" v-for="(preview, i) in previews">
                            <img :src="'/img/' + preview" alt="img non trovata">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../../assets/scss/main.scss" as *;
@use "../../assets/scss/partials/variables.scss" as *;
    // OFFCANVAS
.offcanvas{
    .button_shop{
        background-color: $green;
        padding: 10px 25px;
        border: none;
        color: white;
    }
}
.button_offacnvas{
    position: fixed;
    z-index: 3;
    right: 5px;
    top: 30%;
}

</style>
