<template>


    <div class="static p-3 ">
        <a href="#" class="
            flex flex-col
            items-center
            bg-white
            rounded-lg
            border-2
            shadow-2xl
            md:flex-row md:max-w-2xl
            hover:bg-gray-100
            hover:scale-105
            dark:border-gray-700 dark:bg-gray-800 dark:hover:bg-gray-700
            
        ">
            <img class="
            object-cover
            w-full
            h-96
            rounded-t-lg
            md:h-auto md:w-48 md:rounded-none md:rounded-l-lg
            " src="../assets/images/default.jpg" alt="" />
            <div class="flex flex-col justify-between p-4 leading-normal">
                <p class="
                mb-2
                text-2xl
                font-bold
                tracking-tight
                text-gray-900
                dark:text-white
            ">
                    {{ name }}
                </p>
                <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
                    student ID : {{ studentID }}
                </p>
                <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
                    college : {{ college }}
                </p>
                <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
                    instagram : {{ instagram }}
                </p>
            </div>
        </a>
    </div>


</template>

<script>
export default {
    props: {
        imagePro: {
            type: String,
            default: '../assets/images/ku.png'
        },
        name: {
            type: String,
            default: "No have name"
        },
        studentID: {
            type: String,
            default: "No have studentID"
        },
        college: {
            type: String,
            default: "No have college"
        },
        instagram: {
            type: String,
            default: "No have instagram"
        },
    }
};
</script>