<template >
    <div class="sidenav" style="background-color:#242526">
        <!-- insert image -->
        <div>

            <img class="max-w-full p-7 rounded-full" src="../assets/images/ku.png" alt="image description">

        </div>
        <p class="text-2xl text-center font-extrabold inset-2 text-white">
            Pre-DevCamp
        </p>
        <p class="text-center text-gray-400 font-semibold p-3">
            There will be a tutorial from the basics of HTML CSS Javascript to Frameworks and Databases until you
            can create a project.
        </p>
        <router-link to="/" class="text-white text-center font-semibold p-3">
            Home
        </router-link>
        <router-link to="/profile" class="text-white text-center font-semibold p-3">
            Profile
        </router-link>

    </div>

    <div class="content text-white font-bold">
        <h1 class="text-4xl p-3">CNO Team</h1>
        <div>
            <profile-card 
                imagePro="../assets/images/ong.png" 
                name="Sittipong Hemloun" 
                studentID="6410401183" 
                college="Kasetsart" 
                instagram="sittipongong"
            ></profile-card>
            <profile-card 
                imagePro="../assets/images/ong.png" 
                name="Punnatud Duengkae" 
                studentID="6410406771" 
                college="Kasetsart" 
                instagram="nokkokalderaan"
            ></profile-card>
            <profile-card
                imagePro="../assets/images/ong.png" 
                name="Patinya Saichantadee" 
                studentID="6410406754" 
                college="Kasetsart" 
                instagram="cxld.pty"
            ></profile-card>
        </div>
    </div>


</template>

<script>
import profileCard from '../components/Profile.vue'
export default {
    data() {
        return {
            imagePro: '../assets/images/ong.png',
            name: "Sittipong Hemloun",
            studentID: "6410401183",
            college: "Kasetsart University",
            instagram: "sittipongong",
        }
    },
    components: {
        profileCard
    }
};
</script>
