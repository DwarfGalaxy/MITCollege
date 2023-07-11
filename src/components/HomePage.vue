<template>
    <!-- Header Section -->
    <HomeNav />
    <!-- End of Header Section -->

    <!-- Latest Project Section -->
    <LatestProject />
    <!-- End of Latest Project Section -->

    <!-- About the Company Section -->
    <v-container class="about-company">
        <v-row>
            <!-- div1 -->
            <v-col cols="12" md="6" class="d-flex justify-center align-center">
                <div>
                    <div class="d-flex flex-row align-center choose-div">
                        <v-icon icon="mdi:mdi-comment-edit" class="text-white pa-6 rounded-circle me-3"
                            style="background-color: rgba(93, 185, 88, 1);z-index:100" />
                        <h2 class="text-subtitle-2 font-weight-bold text-capitalize" style="letter-spacing: 1px !important">
                            about the company
                        </h2>
                        <div class="rounded-circle pa-6"></div>
                    </div>
                    <p class="text-h4 mt-4" style="color: rgba(44, 130, 195, 1)">
                        We Believe in Delivering
                    </p>
                    <p class="text-h4" style="color: rgba(44, 130, 195, 1)">THE BEST!</p>
                    <p class="text-justify mt-4">
                        Lorem ipsum dolor sit amet consectetur. Consequat tortor non commodo
                        id sed dolor ut faucibus. Est ultrices eget arcu id at mattis a.
                        Turpis enim feugiat phasellus enim sed tellus tellus. Orci blandit
                        in urna cursus. Cursus vehicula mi auctor cras porttitor lobortis
                        enim enim.
                    </p>
                    <p class="text-justify mt-4">
                        Et sed nulla cursus purus ut adipiscing. Velit sed eu morbi velit
                        diam placerat sed. Vivamus a interdum sed dui tellus gravida
                        sagittis. Rhoncus et lacus habitasse amet molestie est feugiat ac
                        quis. Facilisis volutpat placerat tincidunt nunc neque mattis quis.
                        Lobortis nullam massa.
                    </p>
                    <button class="know-more-btn mt-8 rounded-lg text-white">Know More</button>
                </div>
            </v-col>
            <!-- div2 -->
            <v-col cols="12" md="6" class="d-flex justify-center align-center">
                <div>
                    <v-img src="../assets/images/IMG-20230625-WA0019.jpg" style="clip-path: circle()"></v-img>
                </div>
            </v-col>
        </v-row>
    </v-container>
    <!-- End of About the Company Section -->

    <!-- Our Featured Properties -->
    <FeaturedTestimonials />
    <!-- End of  Our Featured Properties-->

    <!-- About the Company Section-->
    <AboutCompany />
    <!-- End of  About the Company Section -->

    <!-- words from the chairperson Section-->
    <v-container class="mt-14">
        <v-row d-flex>
            <v-col cols="12" md="6" class="d-flex justify-center align-center order-2 order-md-1">
                <div style="clip-path: circle()">
                    <v-img src="../assets/images/IMG-20230625-WA0019.jpg"></v-img>
                </div>
            </v-col>
            <v-col cols="12" md="6" class="d-flex justify-center align-center order-1 order-md-2">
                <div>
                    <div class="d-flex flex-row align-center choose-div">
                        <v-icon icon="mdi:mdi-comment-edit" class="text-white pa-6 rounded-circle me-3"
                            style="background-color: rgba(93, 185, 88, 1);z-index:100" />
                        <h2 class="text-subtitle-2 font-weight-bold " style="letter-spacing: 1px !important">
                            Words from the Chairperson
                        </h2>
                        <div class="rounded-circle pa-6"></div>
                    </div>
                    <p class="text-h4 mt-4" style="color: rgba(44, 130, 195, 1)">
                        Executive Perspective on Real Estate
                    </p>

                    <p class="text-justify mt-4">
                        "Lorem ipsum dolor sit amet consectetur. Cras augue suspendisse
                        pretium non. Eu magna nisi velit elit justo. Id risus tincidunt dui
                        diam faucibus phasellus maecenas lorem nullam. Lorem tempus
                        nec lectus sed. Etiam felis facilisi magna et blandit feugiat. Amet
                        lobortis quis nulla sagittis sodales proin purus. laculis sed auctor
                        condimentum interdum fermentum cras neque.
                        Rhoncus aliquam elementum metus venenatis present scelerisque
                        id scelerisque. Nunc commodo lectus ac neque eu."
                    </p>
                    <h3 class="mt-4 font-weight-medium" style="color:rgba(44, 130, 195, 1) ;letter-spacing: 1px;">Full Name
                    </h3>
                    <p style="color:rgba(107, 107, 107, 1)">Founder & CEO, Legend Investment</p>
                </div>
            </v-col>
        </v-row>
    </v-container>
    <!-- End of  words from the chairperson Section-->

    <!-- Testimonials Section -->
    <v-container class="mt-7">
        <div class="mb-7">
            <div class="d-flex flex-row align-center justify-center  ">
                <div class="testimonials-div">
                    <div class="rounded-circle pa-6 "></div>
                    <v-icon icon="mdi:mdi-comment-edit" class="text-white pa-6 rounded-circle me-3"
                        style="background-color: rgba(44, 130, 195, 1);z-index:100" />
                </div>
                <h2 class="text-subtitle-2 font-weight-bold " style="letter-spacing: 1px !important">
                    Testimonials
                </h2>
            </div>

            <h3 class="text-h4 font-weight-regular mt-3 text-center" style="color:rgba(44, 130, 195, 1);">What Our Clients
                Say</h3>
        </div>
        <!-- carousel -->
        <v-row>
            <v-col cols="12" md="4" v-for="index in 3" :key="index">
                <TestimonialsCard />
            </v-col>
        </v-row>
    </v-container>
    <!-- End of Testimonials Section -->

    <!-- Find your perfect property today section -->
    <v-sheet class="property-section mt-10">
        <v-container class="py-16">
            <div class="d-flex justify-center align-center text-center text-white">
                <div>
                    <h2 class="text-h4 mb-3">Find Your Perfect Property Today</h2>
                    <p class="mb-5">Explore a wide range of premium land options for your next investment or dream project.
                    </p>
                    <v-btn size="x-large" rounded="lg" class="text-capitalize elevation-0 "
                        style="color: rgba(44, 130, 195, 1);">
                        Browse Properties
                    </v-btn>
                </div>
            </div>
        </v-container>
    </v-sheet>
    <!-- End of Find your perfect property today section -->

    <!-- Contact Us Section -->
    <v-sheet class="mt-16 ">
        <h2 class="text-h4 font-weight-regular section-title text-center mb-10">Contact Us</h2>
        <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3532.113144383354!2d85.31311931438604!3d27.717245932704153!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x39eb18202f982789%3A0xc4644cda46fd2621!2sKathmandu%2C%20Nepal!5e0!3m2!1sen!2sus!4v1625268958760!5m2!1sen!2sus"
            width="100%" height="400" style="border:0;" allowfullscreen="" loading="lazy"></iframe>

        <v-container class="d-flex justify-center  contact-us-main-container">
            <div class="elevation-3  form-div rounded-xl bg-white contact-us-container">
                <form action="" class=" py-10 px-7  ">
                    <h3 class="text-h5 mb-3">Get in Touch</h3>
                    <v-row>
                        <v-col cols="6">
                            <v-text-field label="First name" type="name" required variant="outlined"
                                prepend-inner-icon="mdi:mdi-account-outline"></v-text-field>

                        </v-col>
                        <v-col cols="6">
                            <v-text-field label="Phone Number" type="number" required variant="outlined"
                                prepend-inner-icon="mdi:mdi-phone"></v-text-field>
                        </v-col>
                    </v-row>
                    <v-text-field label="Email" type="email" required variant="outlined"
                        prepend-inner-icon="mdi:mdi-email-outline"></v-text-field>

                    <v-textarea label="Write Your Message.." variant="outlined"></v-textarea>

                    <!-- <v-btn type="submit" size="x-large">Submit</v-btn> -->
                    <v-btn type="submit" size="large" rounded="lg" class="text-capitalize elevation-0 text-white px-10 "
                        style="background-color: rgba(93, 185, 88, 1);">
                        Submit
                    </v-btn>
                </form>
                <div class="rounded-b-xl d-flex justify-center align-center py-4 "
                    style="background-color: rgba(44, 130, 195, 1);">
                    <div class="d-flex flex-column  flex-lg-row justify-space-evenly text-white">
                        <div class="d-flex align-center">
                            <v-icon icon="mdi:mdi-map-marker-outline"></v-icon>
                            <p>Kathmandu,Nepal</p>
                        </div>
                        <div class="d-flex align-center mx-0 mx-lg-7 my-4 my-lg-0">
                            <v-icon icon="mdi:mdi-phone"></v-icon>
                            <p>9811761743</p>
                        </div>
                        <div class="d-flex align-center">
                            <v-icon icon="mdi:mdi-email-outline"></v-icon>
                            <p class="ms-1">yubrajkoirala7278@gmail.com</p>
                        </div>
                    </div>
                </div>
            </div>

        </v-container>


    </v-sheet>
    <!-- End of Contact Us Section -->

    <!-- Footer Section -->
    <FooterSection class="mt-0 pt-0" />
    <!-- End of Footer Section -->
</template>
<script setup>
import AboutCompany from './AboutCompany.vue';
import FeaturedTestimonials from './FeaturedTestimonials.vue';
import TestimonialsCard from './TestimonialsCard.vue';
import FooterSection from './FooterSection.vue';
import HomeNav from './HomeNav.vue';
import LatestProject from './LatestProject.vue';


// import PracticeAll from './PracticeAll.vue';
// import { ref } from 'vue';


</script>
<style scoped>
/*   <!-- About the Company Section --> */
.know-more-btn {
    width: 150px;
    height: 46px;
    background-color: rgba(93, 185, 88, 1);
    letter-spacing: 1px;
}

.choose-div,
.testimonials-div {
    position: relative;
}

.choose-div div {
    background-color: rgba(93, 185, 88, 0.4);
    position: absolute;
    left: 0px;
    top: -13px;
}

.about-company {
    position: relative;
    top: -61px;
}

/*   <!-- End of About the Company Section --> */

/* Testimonials Section  */
.testimonials-div div {
    background-color: rgba(44, 130, 195, 0.4);
    position: absolute;
    left: 0px;
    top: -13px;
}

/* End of  Testimonials Section*/

/*  <!-- Find you perfect property today section --> */
.property-section {
    background-image: url("../assets/images/Group 22.png");
    background-repeat: no-repeat;
    background-size: cover;
}

/* End of  Find you perfect property today section*/
.contact-us-main-container {
    position: relative;
}

.contact-us-container {
    position: relative;
    bottom: 116px;
}

@media (min-width:800px) {
    .form-div {
        width: 80%;
    }
}

@media (min-width:1000px) {
    .form-div {
        width: 90%;
    }
}

@media (min-width:1300px) {
    .form-div {
        width: 70%;
    }
}

@media (max-width:800px) {
    .form-div {
        width: 90%;
    }
}

@media (max-width:500px) {
    .form-div {
        width: 95%;
    }
}
</style>
