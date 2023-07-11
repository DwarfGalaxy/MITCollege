<template >
    <v-container class="latest-container">
        <div class="elevation-6 rounded-xl py-4 " style=" background-color: white;">
            <v-row class="d-flex align-center">
                <v-col cols="12" lg="7">
                    <div class="pt-3 pt-lg-0">
                        <h2 class="text-center text-lg-end font-weight-regular text-h4 "
                            style="color: rgba(44, 130, 195, 1);">
                            Latest
                            Projects</h2>
                    </div>
                </v-col>
                <v-col cols="12" lg="5">
                    <div class="mx-10 ">
                        <v-text-field label="Search Properties.." variant="outlined" density="compact" class="mt-4"
                            append-inner-icon="mdi:mdi-magnify"></v-text-field>
                    </div>
                </v-col>
            </v-row>
            <v-row class="px-10">
                <v-col cols="12" lg="4" v-for="index in 3" :key="index">
                    <LatestprojectCard />
                </v-col>
            </v-row>
            <div class="d-flex justify-center justify-lg-end mt-3 me-0 me-lg-9">
                <v-btn variant="text" class="text-capitalize font-weight-bold" style="color: rgba(93, 185, 88, 1);">Explore
                    All
                    Properties</v-btn>
            </div>
        </div>
    </v-container>
</template>
<script setup>
import LatestprojectCard from './LatestprojectCard.vue';
</script>
<style scoped>
.hero-div {
    background: linear-gradient(to bottom, rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.5)), url("../assets/images/herosection.png") no-repeat;
    /* background-image: url("../assets/images/herosection.png"); */
    background-repeat: no-repeat;
    background-size: cover;
    height: 35vh;
    /* height: 100%; */
}

.latest-container {
    position: relative;
    top: -130px;
    z-index: 1000;
    width: 100%;
}
</style>