<template>
    <v-footer class="footer-section d-flex flex-column">
        <v-container class="footer-container">
            <v-row>
                <v-col cols="12" lg="5">
                    <div>
                        <div class="d-flex align-center">
                            <div>
                                <v-img src="../assets/images/footerLogo.png" style="height: 80px;width: 80px;"></v-img>
                            </div>

                            <h2 class="text-white text-h6 text-sm-h5 font-weight-bold ms-3"
                                style="letter-spacing: 1px !important;">
                                Legend
                                Investment </h2>
                        </div>
                        <v-col cols="12" lg="9" class=" ps-0">
                            <div>
                                <p class="text-justify text-white  font-weight-light ">Lorem ipsum dolor sit amet
                                    consectetur.
                                    Gravida mauris lacus id sit. Urna gravida sapien
                                    risus urna. Porttitor non duis praesent
                                    pellentesque facilisis turpis netus. Nisi nibh.
                                    Porttitor non duis praesent pellentesque
                                    facilisis turpis netus. Nisi nibh</p>
                            </div>
                        </v-col>
                        <div>
                            <h3 class="text-white font-weight-regular">Follow us on</h3>
                            <div class="d-flex flex-row mt-3">

                                <v-btn icon="mdi:mdi-twitter" class="text-white" density="compact" href="#"
                                    variant="outlined" size="large">

                                </v-btn>

                                <v-btn icon="mdi:mdi-instagram" class="text-white mx-3" density="compact" href="#"
                                    variant="outlined" size="large">

                                </v-btn>

                                <v-btn icon="mdi:mdi-facebook" class="text-white" density="compact" href="#"
                                    variant="outlined" size="large">

                                </v-btn>
                            </div>
                        </div>
                    </div>
                </v-col>
                <v-col cols="4" lg="2">
                    <div class="mt-lg-16 text-white">
                        <div class="pt-lg-5">
                            <h3 class="text-subtitle-1 font-weight-bold text-lg-h5">Useful Links</h3>
                            <div class="mt-3">
                                <v-btn variant="text"
                                    class=" ps-0 text-capitalize text-body-2 text-lg-subtitle-1 links-btn  " href="#">
                                    <v-icon icon="mdi:mdi-chevron-right"></v-icon>Home
                                </v-btn>
                            </div>
                            <div class="my-2">
                                <v-btn variant="text"
                                    class=" ps-0 text-capitalize text-body-2 text-lg-subtitle-1 links-btn  " href="#">
                                    <v-icon icon="mdi:mdi-chevron-right"></v-icon>About
                                </v-btn>
                            </div>
                            <div class="mt-3">
                                <v-btn variant="text"
                                    class=" ps-0 text-capitalize text-body-2 text-lg-subtitle-1 links-btn  " href="#">
                                    <v-icon icon="mdi:mdi-chevron-right"></v-icon>Propertices
                                </v-btn>
                            </div>
                        </div>

                    </div>
                </v-col>
                <v-col cols="4" lg="2">
                    <div class="mt-lg-16 text-white">
                        <div class="pt-lg-5">
                            <h3 class="text-subtitle-1 font-weight-bold text-lg-h5">Categories</h3>
                            <div class="mt-3">
                                <v-btn variant="text"
                                    class=" ps-0 text-capitalize text-body-2 text-lg-subtitle-1 links-btn  " href="#">
                                    <v-icon icon="mdi:mdi-chevron-right"></v-icon>Category 1
                                </v-btn>
                            </div>
                            <div class="my-2">
                                <v-btn variant="text"
                                    class=" ps-0 text-capitalize text-body-2 text-lg-subtitle-1 links-btn  " href="#">
                                    <v-icon icon="mdi:mdi-chevron-right"></v-icon>Category 2
                                </v-btn>
                            </div>
                            <div class="mt-3">
                                <v-btn variant="text"
                                    class=" ps-0 text-capitalize text-body-2 text-lg-subtitle-1 links-btn  " href="#">
                                    <v-icon icon="mdi:mdi-chevron-right"></v-icon>Category 3
                                </v-btn>
                            </div>
                        </div>

                    </div>
                </v-col>
                <v-col cols="4" lg="3">
                    <div class="mt-lg-16 text-white">
                        <div class="pt-lg-5">
                            <h3 class="  text-subtitle-1 font-weight-bold text-lg-h5">For Contact
                            </h3>
                            <p class="mt-3 text-body-2 text-lg-subtitle-1">Address: Kathmandu, Nepal</p>
                            <p class="my-2 text-body-2 text-lg-subtitle-1">Phone: 9811761743</p>
                            <p style="word-break: break-all;white-space: normal;" class="text-body-2 text-lg-subtitle-1">
                                Email:
                                yubrajkoirala7278@gmail.com</p>
                        </div>

                    </div>
                </v-col>
            </v-row>
        </v-container>
    </v-footer>
    <v-container fluid class="text-medium-emphasis text-center  bg-white ">
        <p>Copyright 2023- All Rights Reserved</p>
    </v-container>
</template>
<script setup></script>
<style scoped>
.footer-section {
    width: 100%;
    background-image: url('../assets/images/Vector\ 4.png');
    background-size: cover;
    background-position: right;
    background-repeat: no-repeat;
    position: relative;
    /* top: -15px; */


}

.footer-container {
    margin-top: 130px;
}

@media(min-width:1678px) {
    .footer-container {
        padding-top: 70px;
    }

}

@media(max-width:608px) {
    .footer-container {
        padding-top: 70px;
    }

}

@media(max-width:487px) {
    .footer-container {
        padding-top: 170px;
    }

}

@media(min-width:571px) and (max-width:1279px) {
    .footer-container {
        padding-top: 170px;
    }
}


.links-btn {
    color: white;
}

.links-btn:hover {
    color: orange;
    background-color: transparent !important;
}
</style>
