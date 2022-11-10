<template>
    <div class="sidenav text-center" style="background-color:#242526;">
        <div>

            <img class="max-w-full p-7 rounded-full animate-[wiggle_1s_ease-in-out_infinite]"
                src="../assets/images/ku.png" alt="image description">

        </div>
        <p class="text-2xl font-extrabold inset-2 text-white">
            Pre-DevCamp
        </p>
        <p class="text-gray-400 font-semibold p-3">
            There will be a tutorial from the basics of HTML CSS Javascript to Frameworks and Databases until you
            can create a project.
        </p>

        <router-link to="/" class="text-white font-semibold p-3">
            <span>
                <font-awesome-icon class="text-white mx-2 hover:text-black" icon="fa-solid fa-house-user" />
                Home
            </span>
        </router-link>
        <router-link to="/profile" class="text-white font-semibold p-3 ">
            <span>
                <font-awesome-icon class="text-white mx-2 hover:text-black" icon="fa-regular fa-address-card" />
                Profile
            </span>
        </router-link>

    </div>

</template>

<script>
export default {
    name: "Navbar",
};
</script>