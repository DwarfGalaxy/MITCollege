<template>
    <!-- Header Section -->
    <PropertiesNav />
    <!-- End of Header Section -->
    <!-- Select Properties Details Section-->
    <v-container class="elevation-24 border-0 mt-5  properties-detail bg-white rounded-lg rounded-ts-0">
        <div class="d-flex btn-div">
            <v-btn size="large" class="text-capitalize pt-4 pb-10 elevation-0 rounded-ts-lg rounded-te-0 rounded-b-0 "
                prepend-icon="mdi:mdi-credit-card-marker-outline" style="color: rgba(44, 130, 195, 1);">Land</v-btn>

            <v-btn size="large" class="text-capitalize pt-4 pb-10  elevation-0 rounded-te-lg rounded-0 "
                prepend-icon="mdi:mdi-home" style="background-color: 
rgba(244, 244, 244, 1);">House</v-btn>
        </div>

        <v-row class=" mx-2 ">
            <v-col cols=" 12" md="3">
                <div>
                    <p class="  font-weight-bold mb-2">Location</p>
                    <v-autocomplete label="Select Location"
                        :items="['California', 'Colorado', 'Florida', 'Georgia', 'Texas', 'Wyoming']" variant="outlined"
                        density="compact" prepend-inner-icon="mdi:mdi-map-marker-outline"
                        append-inner-icon="mdi:mdi-chevron-down"></v-autocomplete>
                </div>
            </v-col>
            <v-col cols="12" md="3" class="py-0 py-md-3">
                <div>
                    <p class=" font-weight-bold mb-2">Area</p>
                    <v-autocomplete label="Select Area"
                        :items="['1000msq-500msq', '1000msq-500msq', '1000msq-500msq', '1000msq-500msq', '1000msq-500msq', '1000msq-500msq']"
                        variant="outlined" density="compact" prepend-inner-icon="mdi:mdi-credit-card-marker"
                        append-inner-icon="mdi:mdi-chevron-down"></v-autocomplete>
                </div>
            </v-col>
            <v-col cols="12" md="3">
                <div>
                    <p class=" font-weight-bold mb-2">Price Range</p>
                    <v-autocomplete label="Select Price Range"
                        :items="['10,000,00-20,00,000', '10,000,00-20,00,000', '10,000,00-20,00,000', '10,000,00-20,00,000', '10,000,00-20,00,000', '10,000,00-20,00,000']"
                        variant="outlined" density="compact" prepend-inner-icon="mdi:mdi-cash"
                        append-inner-icon="mdi:mdi-chevron-down"></v-autocomplete>
                </div>
            </v-col>
            <v-col cols="12" md="3" class=" d-md-flex justify-center align-center">
                <div>
                    <v-btn class="elevation-0 text-capitalize px-10 text-white" size="large"
                        style="background-color: rgba(93, 185, 88, 1);width: 100% !important;">Search</v-btn>
                </div>
            </v-col>
        </v-row>
    </v-container>
    <!-- Select Properties Details Section-->

    <!-- Properties for sales section -->
    <v-container class="sales-properties">
        <v-row>
            <v-col cols="12" sm="4" class="">
                <div class="px-5 py-10 rounded-lg text-left property-category"
                    style="background-color:rgba(239, 239, 239, 1) ;color: rgba(44, 130, 195, 1);">
                    <div>
                        <h3 class="text-black font-weight-medium" style="letter-spacing: 1px;">Property Categories</h3>
                        <v-btn prepend-icon="mdi:mdi-credit-card-marker-outline" variant="text"
                            class="text-capitalize w-100 mt-6 " size="large"
                            style="background-color: rgba(232, 229, 229, 1);">
                            Land
                        </v-btn>
                        <v-btn prepend-icon="mdi:mdi-credit-card-marker-outline" variant="text"
                            class="text-capitalize w-100 mt-4" size="large"
                            style="background-color: rgba(232, 229, 229, 1);">
                            House
                        </v-btn>
                        <v-btn prepend-icon="mdi:mdi-credit-card-marker-outline" variant="text"
                            class="text-capitalize w-100 mt-4" size="large"
                            style="background-color: rgba(232, 229, 229, 1);">
                            Office Space
                        </v-btn>
                        <v-btn prepend-icon="mdi:mdi-credit-card-marker-outline" variant="text"
                            class="text-capitalize w-100 mt-4" size="large"
                            style="background-color: rgba(232, 229, 229, 1);">
                            Apartment
                        </v-btn>
                        <v-btn prepend-icon="mdi:mdi-credit-card-marker-outline" variant="text"
                            class="text-capitalize w-100 mt-4" size="large"
                            style="background-color: rgba(232, 229, 229, 1);">
                            Business
                        </v-btn>


                    </div>
                </div>
            </v-col>
            <v-col cols="12" sm="8">
                <v-row>
                    <v-col cols="12" md="6">
                        <div>
                            <div>
                                <h2 class="text-h4 mb-2" style="color: rgba(44, 130, 195, 1);
;">Properties for Sale</h2>
                                <p>Lorem ipsum dolor sit amet consectetur.</p>
                            </div>
                        </div>
                    </v-col>
                    <v-col cols="12" md="6">
                        <div class="mt-0 mt-md-3">
                            <div class="d-flex flex-row  ">
                                <p class="mt-3 me-3 font-weight-medium">Sort By</p>
                                <v-autocomplete :items="['Average-Price', 'Max-Price', 'Latest-First', 'Highest-Price']"
                                    variant="outlined" density="compact" append-inner-icon="mdi:mdi-chevron-down"
                                    placeholder="Latest First"></v-autocomplete>

                            </div>
                        </div>
                    </v-col>
                </v-row>
                <v-row>
                    <v-col cols="12" lg="6" v-for="index in 6" :key="index">
                        <FeaturedCard class="elevation-4" />
                    </v-col>
                </v-row>
                <div class="d-flex justify-center mt-5" style="color: rgba(44, 130, 195, 1);">
                    <v-pagination v-model="page" :length="5" rounded="0" prev-icon="mdi:mdi-chevron-left"
                        next-icon="mdi:mdi-chevron-right"></v-pagination>
                </div>
            </v-col>
        </v-row>


    </v-container>
    <!-- End of Properties for sales section  -->

    <!-- Footer Section -->
    <FooterSection />
    <!-- End of footer section -->
</template>
<script setup>
import FeaturedCard from './FeaturedCard.vue';
import FooterSection from './FooterSection.vue';
import PropertiesNav from './PropertiesNav.vue';


</script>
<style scoped>
.properties-detail {
    position: relative;
    top: -61px;
    z-index: 9999 !important;
}

.properties-detail .btn-div {
    position: absolute;
    top: -56px;
    left: 0px;
}

@media (max-width:959px) {
    .properties-detail {
        width: 90%;
    }
}

@media(min-width:600px) {
    .property-category {
        position: sticky;
        top: 0px;
    }
}
</style>