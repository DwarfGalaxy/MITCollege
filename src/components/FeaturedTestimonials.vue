<template>
    <v-container class="mt-7">
        <h2 class="section-title text-center text-h4 mb-7 mb-lg-10">Our Featured Properties</h2>
        <!-- for small devices -->
        <v-carousel :continuous="true" :show-arrows="false" hide-delimiter-background delimiter-icon="mdi:mdi-circle"
            class="card-carousel custom" elevation-0>
            <v-carousel-item v-for="index in 6" :key="index">
                <FeaturedCard class="elevation-2" :btnText="text" />
            </v-carousel-item>
        </v-carousel>
        <!-- for large device -->
        <v-row class="tesimonials-card">
            <v-col cols="12" sm="6" lg="4" v-for="index in 6" :key="index">
                <FeaturedCard class="elevation-3" />
            </v-col>
        </v-row>
        <div class="d-flex justify-center mt-7  ">
            <v-btn class=" explore-more-btn text-white text-button text-capitalize" size="large">Explore More</v-btn>
        </div>
    </v-container>
</template>
<script setup>
import FeaturedCard from './FeaturedCard.vue';
</script>
<style scoped>
.explore-more-btn {
    background-color: rgba(93, 185, 88, 1);
}

.explore-more-btn:hover {
    background-color: white;
    color: rgba(93, 185, 88, 1) !important;
}



@media (min-width:430px) {
    .card-carousel {
        display: none;
    }
}

@media (max-width:430px) {
    .tesimonials-card {
        display: none;
    }
}

.v-btn .v-btn__content .v-icon {
    color: rgba(93, 185, 88, 1);
}
</style>