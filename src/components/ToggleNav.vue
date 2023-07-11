<template>
    <v-container class="nav-menu">
        <v-icon :icon="showMobileMenu ? 'mdi:mdi-close' : 'mdi:mdi-menu'" @click="showMenu" class="toggle-icon"></v-icon>
        <div class="nav-content">
            <div class="logo"><v-img src="../assets/images/logoheader.png" class="logo-header"></v-img></div>
            <ul class="nav-items" :class="showMobileMenu ? 'open-menu' : 'closed-menu'">
                <li class=" text-h5 text-sm-subtitle-1 home">Home</li>
                <li class=" text-h5 text-sm-subtitle-1 my-4 about mx-6">About</li>
                <li><v-btn href="#" class="text-white text-capitalize elevation-0 rounded-lg" size="x-large"
                        style="background-color: rgba(93, 185, 88, 1);">Properties</v-btn></li>
            </ul>
        </div>
    </v-container>
</template>
<script setup>
import { ref } from 'vue';

let showMobileMenu = ref(false);

function showMenu() {
    showMobileMenu.value = !showMobileMenu.value;
}


</script>
<style lang="scss" scoped>
.nav-items li {
    position: relative;
    cursor: pointer;
}

.nav-items li::after {
    content: "";
    position: absolute;
    left: 0;
    bottom: -2px;
    width: 0;
    height: 2px;
    // background-color: rgba(93, 185, 88, 1);
    background-color: white;
    transition: width 0.3s ease;
}



.nav-items li:hover::after {
    width: 100%;
}

/* Exclude properties from having the line */
.nav-items li:nth-child(3)::after {
    display: none;
}

.logo-header {
    // height: 200px;
    width: 250px;
}



.nav-content {
    display: flex;
    justify-content: space-between;
    // padding: 0px 30px;
    align-items: center;
}

.nav-items {
    display: flex;
    justify-content: center;
    align-items: center;
    list-style: none;
    margin: 0;
    padding: 0;

    li {
        padding: 0 10px;
    }
}

i {
    display: none;
}

.nav-menu {
    color: white;
}

@media screen and (min-width:768px) {
    .v-container {
        padding: 5px 16px !important;
    }
}

// Mobile version - hidden hamburger menu
@media screen and (max-width: 767px) {


    .nav-menu {
        background-color:
            white;
        color: black !important;
        padding-top: 70px;
        position: absolute;
        width: 100%;
        z-index: 100;
        // box-shadow: -1px 0px 17px -8px rgba(0, 0, 0, 0.75);

    }

    .open-menu {
        opacity: 1;
        height: 200px;
    }



    .closed-menu {
        opacity: 0;
        height: 0;
        padding: 0;
    }

    .nav-content {
        flex-direction: column;
        z-index: 100;
        position: relative;
        transition: all 0.3s ease-out;
    }

    .nav-items {
        flex-direction: column;
        font-size: 2rem !important;
    }


    i {
        display: block;
        text-align: right;
        padding: 0 10px 10px 0;
        position: absolute;
        right: 20px;
        top: 12px;
        font-size: 3rem;
        color: rgba(93, 185, 88, 1);
    }

    .logo {
        position: absolute;
        left: 0px;
        top: -70px;
    }

    .toggle-nav[data-v-342a6878] {
        position: fixed;
        z-index: 9999;
    }
}

@media(max-width:338px) {
    i {
        font-size: 2rem;
        top: 21px;
        right: 5px;
    }
}
</style>