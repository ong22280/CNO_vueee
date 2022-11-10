<template>
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
        <router-link to="/default" class="text-white text-center font-semibold p-3">
            Home
        </router-link>

    </div>
</template>

<script>
export default {
    name: "Navbar",
    data() {
        return {
            image: "../assets/images/ku.png",
            name: "Pre-DevCamp",
            description: "There will be a tutorial from the basics of HTML CSS Javascript to Frameworks and Databases until you can create a project.",
            home: "Home",
        };
    },
};
</script>