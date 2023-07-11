<template>
    <v-carousel :show-arrows="false" hide-delimiter-background class="carousel-container">
        <v-carousel-item v-for="(item, i) in items" :key="i" :src="item.src" cover></v-carousel-item>
        <v-container class="hero-desc">
            <v-row>
                <v-col cols="12" sm="9" md="8" lg="6">
                    <div class="text-white">
                        <h2 class="text-xs-h5 text-sm-h4 text-sm-h3 text-capitalize font-regular">We Believe in
                            Delivering
                        </h2>
                        <h2 class="text-xs-h5 text-sm-h4 text-sm-h3 text-capitalize font-weight-bold mt-1">THE BEST!</h2>
                        <p class="text-xs-subtitle-1 text-sm-h6 font-weight-regular my-2">Explore Your Investment Potential
                            and Transform yours
                            Dreams into Financial Success with Legend Investment.</p>
                        <div class="d-flex flex-row mt-3">

                            <v-btn icon="mdi:mdi-twitter" class="text-white" density="compact" href="#" variant="outlined"
                                size="large">

                            </v-btn>

                            <v-btn icon="mdi:mdi-instagram" class="text-white mx-3" density="compact" href="#"
                                variant="outlined" size="large">

                            </v-btn>

                            <v-btn icon="mdi:mdi-facebook" class="text-white" density="compact" href="#" variant="outlined"
                                size="large">

                            </v-btn>
                        </div>
                    </div>
                </v-col>
            </v-row>
        </v-container>

    </v-carousel>
    <ToggleNav class="toggle-nav" />
</template>
<script setup>
import ToggleNav from './ToggleNav.vue';
let items = [
    {
        src: require('../assets/images/home.jpg'),
    },
    {
        src: require('../assets/images/home.jpg'),
    },
    {
        src: require('../assets/images/home.jpg'),
    },
    {
        src: require('../assets/images/home.jpg'),
    },
]
</script>

<style lang="scss" scoped>
.toggle-nav {
    position: absolute;
}

.carousel-container {
    position: relative;
}

.hero-desc {
    position: absolute;
    top: 25%;
    transform: translateY(-50%);
    // background-color: red;
    left: 51%;
    transform: translateX(-50%);
}

@media(min-width: 600px) and (max-width:639px) {
    .hero-desc {
        top: 18%;
    }
}

.v-carousel-item {
    height: 105vh;
    filter: brightness(50%);
    -webkit-clip-path: polygon(0 0, 80% 0%, 100% 0, 100% 66%, 99% 67%, 50% 96%, 0 69%, 0% 20%);
    clip-path: polygon(0 0, 80% 0%, 100% 0, 100% 66%, 99% 67%, 50% 96%, 0 69%, 0% 20%);
}

@media screen and (min-width:768px) {
    .toggle-nav {
        left: 50%;
        transform: translateX(-50%);
    }
}
</style>