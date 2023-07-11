<template>
    <div class="hero-div text-white " @click="toggleFeatures">
        <div class="ms-4 ">
            <p><v-icon icon="mdi:mdi-map-marker-outline" class="me-1"></v-icon> <span
                    class="font-weight-thin">Location:</span>
                Kathmandu Nepal</p>
            <p class="mt-2"><v-icon icon="mdi:mdi-credit-card-marker-outline" class="me-1"></v-icon><span
                    class="font-weight-thin">Area:</span> 10
                Ropani</p>
        </div>
        <div class="ms-4 show-features">
            <h3 class="text-subtitle-1">Key Features</h3>
            <ul class="ms-5 text-subtitle-2 font-weight-light">
                <li>Pitched Road</li>
                <li>Electricity Facity</li>
                <li>Drainage Facility</li>
                <li>Open Area and Playground</li>
            </ul>
        </div>
        <div class="d-flex justify-end">
            <v-btn variant="text" class="text-white text-capitalize" append-icon="mdi:mdi-arrow-right">View
                Details</v-btn>
        </div>

    </div>
</template>
<script setup>

</script>
<style scoped>
.hero-div {
    display: flex;
    justify-content: end;
    flex-direction: column;
}

.show-features {
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.3s ease;
}

.hero-div:hover .show-features {
    max-height: 200px;
    transition: max-height 1.8s ease;
}

@media (max-width:650px) {
    .hero-div:after .show-features {
        max-height: 200px;
        transition: max-height 0.3s ease;
    }
}
</style>