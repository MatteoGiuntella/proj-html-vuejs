<script>
import { arrow } from '@popperjs/core';

export default {
    data() {
        return {
            
        };
    },
    props:{
        widgetNumber: Array
    },
    methods: {

    }
}
</script>

<template>
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
</template>

<style lang="scss" scoped>
@use "../../assets/scss/main.scss" as *;
@use "../../assets/scss/partials/variables.scss" as *;
.little_container{
        display: flex;
        justify-content: center;
        align-items: center;
        width: 900px;
        margin: 0 auto;
        .number_section_3{
            display: flex;
            justify-content: center;
            color: $green;
            font-size: 2.7em;
            font-weight: 600;
        }
        .info_section_3{
            display: flex;
            justify-content: center;
            color: $purple;
        }
    
    }

</style>
