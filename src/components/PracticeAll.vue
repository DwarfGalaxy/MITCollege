<template>
    <v-container>
        <vueper-slides class="no-shadow" :visible-slides="3" slide-multiple :gap="3" :slide-ratio="1 / 4"
            :dragging-distance="200" :breakpoints="{ 900: { visibleSlides: 1, slideMultiple: 2 } }">
            <vueper-slide v-for="(slide, i) in slides" :key="i" :title="slide.title" :content="slide.content">
            </vueper-slide>
            <!-- <TestimonialsCard v-for="i in 10" :key="i" /> -->
        </vueper-slides>
    </v-container>
</template>
<script setup>
import { VueperSlides, VueperSlide } from 'vueperslides'
import 'vueperslides/dist/vueperslides.css';
// import TestimonialsCard from './TestimonialsCard.vue';
// import TestimonialsCard from './TestimonialsCard.vue';

const slides = [
    {
        title: 'Slide #1',
        content: 'Slide 1 content.'
    },
    {
        title: 'Slide #2',
        content: 'Slide 2 content.'
    },
    {
        title: 'Slide #1',
        content: 'Slide 1 content.'
    },
    {
        title: 'Slide #2',
        content: 'Slide 2 content.'
    },
    {
        title: 'Slide #1',
        content: 'Slide 1 content.'
    },
    {
        title: 'Slide #2',
        content: 'Slide 2 content.'
    }
]
</script>
<style></style>
