<template>
    <!-- Header Section -->
    <div style="background-color: 
rgba(197, 245, 194, 1);">
        <ToggleNavVue style="color: rgba(44, 130, 195, 1);" />
    </div>
    <!-- End of Header Section -->

    <!-- Palace Project Bhakatapur Section  -->
    <v-container class="palace-bktpur-container">
        <div class="d-md-flex flex-row  justify-space-between align-center ">
            <div>
                <h2 class="text-h5 text-md-h4 font-weight-medium">Palase Project Bhaktapur</h2>
                <div class="d-flex mt-4 mb-6 text-medium-emphasis">
                    <div class="d-flex align-center font-weight-medium">
                        <v-icon icon="mdi:mdi-map-marker-outline"></v-icon>
                        <p class="me-5 ">Palase, Bhakatapur</p>
                    </div>

                    <p>Posted on: 23rd June,2023</p>
                </div>


            </div>
            <div class="mb-5 mb-md-0">
                <p class="text-h5 font-weight-bold" style="color: rgba(44, 130, 195, 1);">Rs. 10,00,000</p>
            </div>
        </div>
        <v-row>
            <v-col cols="12" md="8">
                <div>
                    <v-img src="../assets/images/land1.png"></v-img>
                </div>
            </v-col>
            <v-col cols="12" md="4">
                <v-row>
                    <v-col cols="12">
                        <div>
                            <v-img src="../assets/images/land2.png" class="rounded-lg"></v-img>
                        </div>
                    </v-col>
                    <v-col cols="12">
                        <div>
                            <v-img src="../assets/images/land6.png" class="rounded-lg"></v-img>
                        </div>
                    </v-col>
                </v-row>
            </v-col>
            <v-col cols="12" md="4">
                <div>
                    <v-img src="../assets/images/land3.png" class="rounded-lg"></v-img>
                </div>
            </v-col>
            <v-col cols="12" md="4">
                <div>
                    <v-img src="../assets/images/land4.png" class="rounded-lg"></v-img>
                </div>
            </v-col>
            <v-col cols="12" md="4">
                <div class="last-div">
                    <v-img src="../assets/images/land5.png" class="rounded-lg"></v-img>
                    <v-btn variant="outlined" class="text-white text-capitalize rounded-lg" size="large">View All
                        Photos</v-btn>
                </div>
            </v-col>
        </v-row>
    </v-container>
    <!-- End of Palace  Project Bhakatapur Section-->

    <!-- Palace Project Details Section -->
    <v-container>
        <v-row class="d-flex justify-center ">
            <v-col cols="12" md="8">
                <div>
                    <v-expansion-panels v-model="panel" :disabled="disabled" multiple>
                        <!-- expansion panel 1 -->
                        <v-expansion-panel style="background-color: rgba(244, 249, 252, 1);;">
                            <v-expansion-panel-title class="font-weight-bold" expand-icon="mdi:mdi-chevron-down"
                                collapse-icon="mdi:mdi-chevron-up">Description</v-expansion-panel-title>
                            <v-expansion-panel-text>
                                <p class="text-justify text-high-emphasis ">Beautiful, updated,
                                    ground level Co-op
                                    apartment in the desirable
                                    Bay Terrace
                                    neighborhood. This
                                    home features hardwood floors throughout, brand new bathrooms, newer EK, modern
                                    front-load
                                    washer/dryer, full dining room, large living area, 3 spacious bedrooms and plenty of
                                    storage. Master
                                    bedroom includes both a standard closet and custom closet wall unit. Large windows face
                                    many
                                    directions for tons of natural light.</p>
                            </v-expansion-panel-text>
                        </v-expansion-panel>

                        <!-- expansion panel 2 -->
                        <v-expansion-panel class="mt-9" style="background-color: rgba(244, 249, 252, 1);">
                            <v-expansion-panel-title class="font-weight-bold" expand-icon="mdi:mdi-chevron-down"
                                collapse-icon="mdi:mdi-chevron-up">Features</v-expansion-panel-title>
                            <v-expansion-panel-text>
                                <v-row>
                                    <v-col cols="12" md="4">
                                        <div class="d-flex align-center">
                                            <v-icon icon="mdi:mdi-road-variant" style="color: rgba(44, 130, 195, 1)"
                                                class="me-3"></v-icon>
                                            <p class=" text-medium-emphasis">8 Meter Pitched Road</p>
                                        </div>
                                    </v-col>
                                    <v-col cols="12" md="8">
                                        <div class="d-flex align-center ">
                                            <v-icon icon="mdi:mdi-cable-data" style="color: rgba(44, 130, 195, 1)"
                                                class="me-3"></v-icon>
                                            <p class=" text-medium-emphasis">Electricity Facility</p>
                                        </div>
                                    </v-col>
                                    <v-col cols="12" md="4">
                                        <div class="d-flex align-center">
                                            <v-icon icon="mdi:mdi-pipe" style="color: rgba(44, 130, 195, 1)"
                                                class="me-3"></v-icon>
                                            <p class=" text-medium-emphasis">Drainage Facility</p>
                                        </div>
                                    </v-col>
                                    <v-col cols="12" md="8">
                                        <div class="d-flex align-center">
                                            <v-icon icon="mdi:mdi-water-pump" style="color: rgba(44, 130, 195, 1)"
                                                class="me-3"></v-icon>
                                            <p class=" text-medium-emphasis">Water Supply</p>
                                        </div>
                                    </v-col>
                                </v-row>
                            </v-expansion-panel-text>
                        </v-expansion-panel>

                        <!-- expansion panel 3 -->
                        <v-expansion-panel class="mt-9" style="background-color: rgba(244, 249, 252, 1);">
                            <v-expansion-panel-title class="font-weight-bold" expand-icon="mdi:mdi-chevron-down"
                                collapse-icon="mdi:mdi-chevron-up">Overview</v-expansion-panel-title>
                            <v-expansion-panel-text>
                                <v-row class="d-flex justify-space-around">
                                    <v-col cols="6" md="3">
                                        <div>
                                            <h3 class="font-weight-regular text-subtitle-1">Price:</h3>
                                            <p class="font-weight-medium">Rs. 100000</p>
                                        </div>
                                    </v-col>
                                    <v-col cols="6" md="3" class="text-center text-md-start">
                                        <div>
                                            <h3 class="font-weight-regular text-subtitle-1">Area</h3>
                                            <p class="font-weight-medium">1000 mt sq</p>
                                        </div>
                                    </v-col>
                                    <v-col cols="6" md="3">
                                        <div>
                                            <h3 class="font-weight-regular text-subtitle-1">Kind of Property</h3>
                                            <p class="font-weight-medium">Plotting Land</p>
                                        </div>
                                    </v-col>
                                    <v-col cols="6" md="3" class="text-center">
                                        <div>
                                            <h3 class="font-weight-regular text-subtitle-1">Facing</h3>
                                            <p class="font-weight-medium">South</p>
                                        </div>
                                    </v-col>
                                </v-row>

                            </v-expansion-panel-text>
                        </v-expansion-panel>


                        <!-- expansion panel 4 -->
                        <v-expansion-panel class="mt-9 " style="background-color: rgba(244, 249, 252, 1) !important;">
                            <v-expansion-panel-title class="font-weight-bold" expand-icon="mdi:mdi-chevron-down"
                                collapse-icon="mdi:mdi-chevron-up">Address</v-expansion-panel-title>
                            <v-expansion-panel-text>
                                <p><span class="font-weight-medium">Tole:</span> Palase</p>
                                <p><span class="font-weight-medium">Address:</span> Palase</p>
                                <p><span class="font-weight-medium">City:</span> Bhaktapur</p>
                                <p><span class="font-weight-medium">District:</span> Bhaktapur</p>
                                <p><span class="font-weight-medium">State:</span> Bagmati Pradesh</p>
                            </v-expansion-panel-text>
                        </v-expansion-panel>

                        <!-- expansion panel 5 -->
                        <v-expansion-panel class="mt-9 " style="background-color: rgba(244, 249, 252, 1);">
                            <v-expansion-panel-title class="font-weight-bold" expand-icon="mdi:mdi-chevron-down"
                                collapse-icon="mdi:mdi-chevron-up">Additional Details</v-expansion-panel-title>
                            <v-expansion-panel-text>
                                <p><span class="font-weight-medium">Property ID:</span> 12925</p>
                                <p><span class="font-weight-medium">Facing Direction (Mohada):</span> South</p>
                                <p><span class="font-weight-medium">Total Price of the property:</span> Rs.10,00,000</p>
                                <p><span class="font-weight-medium">Posted on:</span> 17 June 2023</p>

                            </v-expansion-panel-text>
                        </v-expansion-panel>

                        <!-- expansion panel 6 -->
                        <v-expansion-panel class="mt-9" style="background-color: rgba(244, 249, 252, 1);">
                            <v-expansion-panel-title class="font-weight-bold" expand-icon="mdi:mdi-chevron-down"
                                collapse-icon="mdi:mdi-chevron-up">Video</v-expansion-panel-title>

                            <v-expansion-panel-text>
                                video

                            </v-expansion-panel-text>
                        </v-expansion-panel>

                    </v-expansion-panels>
                </div>
            </v-col>
            <v-col cols="12" md="4">
                <div>
                    <div class="map-container">
                        <iframe
                            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3533.968716736282!2d85.31764531506253!3d27.71724553264703!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x39eb19120a8e646b%3A0x52f5c105d81cc291!2sKathmandu%2044600%2C%20Nepal!5e0!3m2!1sen!2sus!4v1624147936652!5m2!1sen!2sus"
                            width="100%" height="100%" frameborder="0" style="border:0" allowfullscreen></iframe>
                    </div>
                </div>
                <div class="elevation-10 rounded-lg py-7 mt-10">
                    <div class="d-flex justify-center align-center flex-column">
                        <div class="d-flex align-center">
                            <v-img src="../assets/images/logo.png" style="height: 60px;width: 60px;"></v-img>
                            <p class="ms-4 font-weight-medium">Legend Investment</p>
                        </div>
                        <div class="d-flex justify-center align-center flex-column mt-5">
                            <div class="d-flex align-center">
                                <v-btn class="elevation-0 text-capitalize text-white px-10 rounded-lg"
                                    style="background-color: rgba(93, 185, 88, 1);" prepend-icon="mdi:mdi-phone"
                                    size="large">Call
                                    Now</v-btn>
                                <v-btn icon="mdi:mdi-email-outline" variant="outlined"
                                    style="color:rgba(93, 185, 88, 1);border: 2px solid;" class="ms-4 text-subtitle-1"
                                    size="small">
                                </v-btn>

                            </div>
                        </div>
                    </div>
                </div>

                <div class="mt-10 d-flex align-center">
                    <input type="checkbox" class="me-2" style="height: 25px; width: 25px;cursor: pointer;"
                        v-model="showForm" @click="formClicked()" id="interested">
                    <label for="interested" style="cursor: pointer;">I am Interested</label>
                </div>
                <div :style="{ display: showForm ? 'block' : 'none' }"
                    class="elevation-10 mt-7 rounded-lg px-5 py-7 form-div">
                    <div>
                        <v-form>
                            <h2 class="font-weight-medium text-h6 mb-4">Enquiry Form</h2>
                            <v-text-field label="Full Name" required variant="outlined" density="compact"
                                prepend-inner-icon="mdi:mdi-account-outline" type="text" class="text-medium-emphasis"
                                v-model="fullName"></v-text-field>
                            <v-text-field label="Phone Number" required variant="outlined" density="compact"
                                prepend-inner-icon="mdi:mdi-phone-outline" type="number" class="text-medium-emphasis"
                                v-model="phoneNumber"></v-text-field>
                            <v-text-field label="Email" required variant="outlined" density="compact"
                                prepend-inner-icon="mdi:mdi-email-outline" type="email" class="text-medium-emphasis"
                                v-model="emailAddress"></v-text-field>

                            <v-textarea label="Write your Message" auto-grow variant="outlined" rows="3"
                                class="text-medium-emphasis " type="text" v-model="message"></v-textarea>

                            <v-btn class="elevation-0  w-100 text-capitalize text-white text-subtitle-1"
                                style="background-color: rgba(93, 185, 88, 1);;" size="large">Submit
                                Information</v-btn>

                        </v-form>

                    </div>
                </div>
                <div class=" mt-10">
                    <div>
                        <v-row class="d-flex align-center" v-for="index in 4" :key="index">
                            <v-col cols="6">
                                <v-img src="../assets/images/img1.png" class="rounded-lg"></v-img>
                            </v-col>
                            <v-col cols="6">
                                <div>
                                    <p class="font-weight-bold">Anandalava Resort
                                        for Sale</p>
                                    <div class="d-flex flex-row align-center text-medium-emphasis text-subtitle-2 mt-2">
                                        <v-icon icon="mdi:mdi-map-marker-outline"></v-icon>
                                        <p>Damauli</p>
                                    </div>
                                    <p class=" me-3 text-center rounded-lg mt-2 py-1"
                                        style="background-color: rgba(192, 248, 189, 1);">10 Lakh/
                                        AANA</p>
                                </div>
                            </v-col>

                        </v-row>

                    </div>
                </div>
            </v-col>
        </v-row>
    </v-container>
    <!-- End of Palace Project Details Section -->

    <!-- Footer Section -->
    <FooterSection />
    <!-- End of Footer Section -->
</template>
<script setup>
import FooterSection from './FooterSection.vue';
import ToggleNavVue from './ToggleNav.vue';
import { ref } from 'vue';

let panel = ref([0, 1, 2, 3, 4, 5]);
let showForm = ref(false);
const formClicked = () => {
    showForm.value = !showForm.value;
}

// video

</script>
<style scoped>
.palace-bktpur-container {
    margin-top: 2rem;
}

@media(max-width:768px) {
    .palace-bktpur-container {
        margin-top: 6rem;
    }
}

.last-div {
    position: relative;
}

.last-div .v-btn {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

.map-container {
    height: 360px;
    width: 100%;
}

/* video */
</style>