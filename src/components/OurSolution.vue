<template>
    <div class="solution" id="our-solution">
        <div class="container">
            <div class="row justify-content-between solution__row">
                <div class="col-md-4 solution__col align-self-center">
                    <h1 class="solution__col--header">OUR SOLUTION</h1>
                    <p class="solution__col--title">
                        <span class="solution__col--desc">We Buy From </span>
                        <span class="solution__col--desc">Cooperatives, & Sell To </span>
                        <span class="solution__col--desc">Wholesalers & Industries</span>
                    </p>
                    <div class="solution__cta">
                        <a href="https://drive.google.com/file/d/1RmQeZb6VETZQPcU6bjapUEz5vmJMhTft/view"  download target="_blank">
                            <button  type="submit"  class="solution__cta--btn solution__cta--button">Join our Mission</button>
                        </a>
                    </div>
                </div>
                <div class="col-md-8">
                    <div class="row gx-5 justify-content-evenly">
                        <div class="col-md-5 solution__col">
                            <div class="card solution__card h-100 mb-3" style="max-width: 35rem;">
                                <div class="card-body solution__card-body">
                                    <div class="solution__card-img">
                                        <img src="~@/assets/images/img_1/crops.png" class="" alt="..."  width="100">
                                        
                                    </div>
                                    <h5 class="card-title solution__card--title">Improved species of crops. </h5>
                                    <p class="card-text solution__card--text">
                                        <span class="solution__col--sub-text">We help farmers reduce their cost </span>
                                        <span class="solution__col--sub-text">of production by developing crop </span>
                                        <span class="solution__col--sub-text">varieties with high grain potential </span>
                                        <span class="solution__col--sub-text">and directly offtaking from them at </span>
                                        <span class="solution__col--sub-text">good prices. </span>
                                    </p>
                                </div>
                            </div>
                        </div>
                        <div class="col-md-5 solution__col">
                            <div class="card solution__card h-100 mb-3" style="max-width: 35rem;">
                                <div class="card-body solution__card-body">
                                    <div class="solution__card-img">
                                        <img src="~@/assets/images/img_1/food.png" class="" alt="..." width="100">
                                    </div>
                                    <h5 class="card-title solution__card--title">Healthier finished foods.</h5>
                                    <p class="card-text solution__card--text">
                                        <span class="solution__col--sub-text">In response to the inappropriate </span>
                                        <span class="solution__col--sub-text">processing and preservation of farm </span>
                                        <span class="solution__col--sub-text">produce, we produce high quality </span>
                                        <span class="solution__col--sub-text">cassava and maize flours, which will </span>
                                        <span class="solution__col--sub-text">be processed and packaged in </span>
                                        <span class="solution__col--sub-text">compliance with required hygiene </span>
                                        <span class="solution__col--sub-text">standards using modern machines </span>
                                        <span class="solution__col--sub-text">and relevant technology.</span>
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">


</script>

<style lang="scss" scoped>
@import "@/sass/variable.scss";
@import "@/sass/mixin.scss";

.solution {
    padding: 4rem 0;


    &__col {
        padding: 4rem 0;
        font-family: 'Inter';
        font-style: normal;

        &--header{
            color: $color-primary;
            font-weight: map-get($font-weights, medium);
            padding-bottom: .5rem;
            font-size: $font-sm;
        }

        &--title{
            padding-bottom: 2rem;
            display: block;
        }

        &--desc{
            color: $color-deep-green;
            font-size: $font-md;
            font-weight: map-get($font-weights, medium);
            padding-bottom: 1.5rem;
        }
    }

    &__row {
        padding: 4rem 0;
    }

    &__card {
        box-shadow: 0px 4px 20px rgba(12, 53, 15, 0.2);
        border-radius: 10px;

        
        &--title {
            padding-top: 2rem;
            color:  $color-deep-green;
            font-weight: map-get($font-weights, bold);
            font-size: $font-sm;
        }

        // &--img {
        //     width: 50%;
        // }
    }

    &--text {
        padding-top: 2rem;
    }

    &--sub-text {
        display: block;
        font-weight: map-get($font-weights, bold);
        font-size: $font-sm;
    }

    &__card-body {
        padding: 2.5rem 2.5rem;
    }
    
    &__cta {

        @include cta;
    }
}

/* Extra small devices (phones, 600px and down) */

@media only screen and (max-width: 600px) {
    .solution {
        padding: 0rem .5rem;

        &__col {
            padding-top: 0rem;

            &--header{
                font-size: $font-xsm;
            }

            &--desc{
                font-size: $font-xrg;
            }
        }

        &__row {
            padding: 1rem;
        }

        &__card-body {
            padding: 2rem 2rem;
        }

        &__cta {

            @include cta;
        }
    }
}
</style>