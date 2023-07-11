<template>
    <div class="elevation-5 rounded-lg pa-4 card-container">
        <div>
            <v-icon icon="mdi:mdi-home-account" class="text-white pa-5 rounded-lg  me-3 text-h4"
                style="background-color: rgba(44, 130, 195, 0.9)" />
            <p class="font-weight-bold mt-4 mb-2 card-title">01. Property
                Insurance</p>
            <p class="text-justify card-desc">
                Lorem ipsum dolor sit amet
                consectetur. Consequat tortor
                non commodo id sed dolor ut
                faucibus. Est ultrices eget arcu id
                at mattis a. Turpis enim feugiat<span v-if="read">Managed Land Development Project and
                    Housing Area
                    constructed by
                    Green Village</span>
            </p>
            <div class="read-more-btn text-center mt-3">
                <btn v-on:click="readMore">{{
                    !read ? `Read More` : "Read Less"
                }}</btn>
            </div>
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
.read-more-btn {
    cursor: pointer;
    color: rgba(44, 130, 195, 1);
}

.card-title {
    color: rgba(44, 130, 195, 1);
}

.card-desc {
    color: rgba(105, 105, 109, 1);
    font-size: 14px;
}

.card-container {
    transition: background-color 1.4s;
}

.card-container:hover {
    background-color: rgba(44, 130, 195, 1);
    color: white !important;
}

.card-container:hover p,
.card-container:hover .read-more-btn {
    color: white;
}
</style>