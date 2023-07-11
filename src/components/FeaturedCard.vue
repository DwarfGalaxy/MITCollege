<template>
    <div class=" pb-4  rounded-lg">
        <div class="image-container rounded-t-lg"><v-img src="../assets/images/palaase.png"></v-img></div>
        <div class="d-flex justify-space-between align-center  mx-3 ">
            <div>
                <p class="font-weight-bold mt-3 mb-1">
                    Palase Project
                    Bhaktapur</p>
                <div class="d-flex align-center ">
                    <v-icon icon="mdi:mdi-map-marker-outline" style="color: rgba(44, 130, 195, 1); font-size: 20px;" />
                    <p style="color:rgba(110, 110, 113, 1);font-size: 14px;">Palase, Bhaktapur</p>
                </div>
            </div>
            <div>
                <p class="font-weight-bold" style="color: rgba(44, 130, 195, 1)">
                    Rs. 20,000,00
                </p>
            </div>
        </div>
        <div class=" mx-3">
            <p class="text-justify" style="color:rgba(105, 105, 109, 1);font-size: 14px;">
                Managed Land Development Project and Housing Area constructed by
                Green Village <span v-if="read">Managed Land Development Project and Housing Area
                    constructed by
                    Green Village</span>
                <span v-if="!read">...</span> <span style="cursor: pointer;color: rgba(44, 130, 195, 1)"
                    v-on:click="readMore">{{
                        !read ? "Read More" : "Read Less"
                    }}</span>
            </p>
        </div>

        <div class="d-flex justify-space-between mx-3 mt-4">
            <div class="d-flex align-center" style="font-size: 14px;">
                <v-icon icon="mdi:mdi-bus" style="color: rgba(44, 130, 195, 1);" />
                <p class="ms-2">8 Meter Pitched Road</p>
            </div>
            <div class="d-flex align-center" style="font-size: 14px;">
                <v-icon icon="mdi:mdi-credit-card-marker-outline" style="color: rgba(44, 130, 195, 1);" />
                <p class="ms-2">10 Ropani</p>
            </div>
        </div>
        <div class="d-flex aligh-center mx-3 my-4" style="font-size: 14px;">
            <v-icon icon="mdi:mdi-water-pump" style="color: rgba(44, 130, 195, 1);" />
            <p class="ms-2">Electricity, Drainage, Water Facilities</p>
        </div>
        <div class="d-flex justify-end mx-3">
            <button class="view-details-btn rounded-lg px-3 py-2">View Details</button>
        </div>
    </div>
</template>
<script setup>
import { ref } from 'vue';

let read = ref(false);
function readMore() {
    return read.value = !read.value;
}
</script>
<style scoped>
.view-details-btn {
    color: rgba(93, 185, 88, 1);
    border: 1px solid rgba(93, 185, 88, 1);
    transition-duration: 1s;
}

.view-details-btn:hover {
    color: white;
    background-color: rgba(93, 185, 88, 1);
}

.image-container {
    overflow: hidden;
    cursor: pointer;
}

.image-container img {
    transition: transform 0.3s ease;
}

.image-container:hover img {
    transform: scale(1.2);
}
</style>