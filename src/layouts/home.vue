<template>
    <div class="sidenav text-center" style="background-color:#242526;">
        <div>

            <img class="max-w-full p-7 rounded-full animate-[wiggle_1s_ease-in-out_infinite]" src="../assets/images/ku.png" alt="image description">

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

    <div class="content p-8 object-center">

        <div>
            <h1
                class="mb-4 text-4xl font-extrabold tracking-tight leading-none text-gray-900 md:text-5xl lg:text-6xl dark:text-white">
                Bachelor of Science Program in Computer Science</h1>
            <p class="mb-6 text-lg lg:text-xl sm:px-16 text-gray-400 font-semibold p-3">
                Here at
                Flowbite we focus on markets where technology, innovation, and capital can unlock long-term value and
                drive
                economic growth.
            </p>

            <h2 class="mb-2 text-3xl font-semibold text-gray-900 dark:text-white">Course format :</h2>
            <ol class="space-y-1 max-w-full list-decimal list-inside mb-6 text-lg lg:text-xl sm:px-16  text-gray-400 font-semibold p-3 " >
                <li>
                    <span class="font-semibold text-gray-900 dark:text-white">Format and type of course</span> 4-year Undergraduate Program (Academic)
                </li>
                <li>
                    <span class="font-semibold text-gray-900 dark:text-white">language</span> Thai and English
                </li>
                <li>
                    <span class="font-semibold text-gray-900 dark:text-white">admission</span> Accepting both Thai and international students
                </li>
                <li>
                    <span class="font-semibold text-gray-900 dark:text-white">cooperation with other institutions</span> specific course of the institute.
                </li>
                <li>
                    <span class="font-semibold text-gray-900 dark:text-white">Graduation to graduates</span> Grants only one degree
                </li>
            </ol>




        </div>
        <div class="">
            <h1
                class="mb-2 mx-6 text-1xl font-extrabold tracking-tight leading-none text-gray-900 md:text-3xl lg:text-1xl dark:text-white">
                ABOUT CNC
            </h1>
            <iframe class="m-6" width="560" height="315"
                src="https://www.youtube.com/embed/ixzAQw4ZqXk?autoplay=1&mute=1" title="YouTube video player"
                frameborder="2"
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                allowfullscreen></iframe>

        </div>


    </div>

</template>

<script>
export default {

}
</script>

<style>

</style>