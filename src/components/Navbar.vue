<template>
    <div class="sidenav" style="background-color:#242526">
        <div>

            <img class="max-w-full p-7 rounded-full" src="../assets/images/ku.png" alt="image description">

        </div>
        <p class="text-2xl text-center font-extrabold inset-2 text-white">
            {{ name }}
        </p>
        <p class="text-center text-gray-400 font-semibold p-3">
            {{ description }}
        </p>
        <router-link to="/" class="text-white text-center font-semibold p-3">
            {{ home }}
        </router-link>
        <router-link to="/profile" class="text-white text-center font-semibold p-3">
            {{ profile }}
        </router-link>
    </div>
</template>

<script>
export default {
    props: {
        name: {
            type: String,
            default: 'Pre-DevCamp'
        },
        description: {
            type: String,
            default: 'There will be a tutorial from the basics of HTML CSS Javascript to Frameworks and Databases until you can create a project.'
        },
        home: {
            type: String,
            default: 'Home'
        },
        profile: {
            type: String,
            default: 'Profile'
        }
    }
};
</script>