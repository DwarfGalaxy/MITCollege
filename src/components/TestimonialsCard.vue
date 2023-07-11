<template>
    <v-card class=" px-9 pt-12 pb-6 rounded-xl elevation-3">
        <div class="card-section-div">
            <v-img src="../assets/images/Vector.png" class="card-semicolon" style="height: 30px; width: 30px;"></v-img>
            <p class="text-justify">Lorem ipsum dolor sit amet consectetur.
                Consequat tortor
                non commodo id sed dolor ut faucibus. Est ultrices get arcu
                id at mattis a. Turpis enim feugiat phasellus enim sed tellus
                tellus. Orci blandit in urna cursus. Cursus vehicula mi auctor mi auctor</p>
            <v-img src="../assets/images/Vector2.png" style="height: 30px; width: 30px;"
                class="card-semicolon-buttom"></v-img>
            <div class="d-flex align-center flex-row justify-start ">
                <div class="mt-5" style="height: 90px;width: 90px;">
                    <v-img src="../assets/images/348435422_1624113134757133_9178258497192085427_n.jpg"
                        style="clip-path: circle();"></v-img>
                </div>

                <div>
                    <p class="font-weight-bold">Jonh Doe</p>
                    <p class="text-blue-grey-darken-1 text-subtitle-2">CEO, ABC Company</p>
                </div>
            </div>
        </div>
    </v-card>
</template>
<script setup></script>
<style scoped>
.card-section-div {
    position: relative;
}

.card-semicolon {
    position: absolute;
    top: -19px;
    left: -30px
}

.card-semicolon-buttom {
    position: absolute;
    bottom: 98px;
    right: -2px;
}
</style>