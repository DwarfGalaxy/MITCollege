<template>
    <v-sheet class="properties-nav">
        <ToggleNav />
        <div class="properties-div">
            <div class="text-white text-center">
                <h1 class="text-h4 text-sm-h3 font-weight-bold">Properties Listing</h1>
                <p class="text-h6 text-sm-h5 mt-6">View the collection of featured listings and properties for sale.
                </p>
            </div>
        </div>
    </v-sheet>
</template>
<script setup>
import ToggleNav from './ToggleNav.vue';


</script>
<style scoped>
.properties-nav {
    background: linear-gradient(to bottom, rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.5)), url("../assets/images/image.png") no-repeat;
    background-size: cover;
    height: 90vh;
}

.properties-nav {
    position: relative;
}

.properties-div div {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

@media screen and (max-width: 767px) {
    .properties-nav {
        height: 80vh;
    }
}

@media screen and (max-width: 500px) {
    .properties-div div {
        left: 0%;
        transform: translate(0%, -50%);
    }

    .properties-nav {
        height: 70vh;
    }
}
</style>