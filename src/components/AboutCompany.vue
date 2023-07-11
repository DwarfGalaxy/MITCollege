<template>
    <v-container class="mt-7 about-container">
        <v-row>
            <v-col cols="12" lg="6" class="d-flex justify-center align-center">
                <div>
                    <div class="d-flex flex-row align-center choose-div">
                        <v-icon icon="mdi:mdi-comment-edit" class="text-white pa-6 rounded-circle me-3"
                            style="background-color: rgba(44, 130, 195, 1);z-index:100" />
                        <h2 class="text-subtitle-2 font-weight-bold text-capitalize" style="letter-spacing: 1px !important">
                            why choose us
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
                </div>
            </v-col>
            <v-col cols="12" lg="6" d-flex justify-center align-center>
                <v-row>
                    <v-col cols="6" v-for="index in 4" :key="index">
                        <ChooseusCard />
                    </v-col>
                </v-row>
            </v-col>

        </v-row>
    </v-container>
</template>
<script setup>
import ChooseusCard from './ChooseusCard.vue';

</script>
<style scoped>
.choose-div {
    position: relative;
}

.choose-div div {
    background-color: rgba(44, 130, 195, 0.4);
    position: absolute;
    left: 0px;
    top: -13px;
}
</style>