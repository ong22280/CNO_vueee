<template>

    <RouterView />
</template>

<!-- <script>
import Navbar from './components/Navbar.vue'
export default {
    name: 'App',
    components: {
        Navbar,
    },
}
</script> -->

<style>
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family: Arial, Helvetica, sans-serif;
    background-image: url('src/assets/images/bg.png');

}

/* Style the side navigation */
.sidenav {
    height: 100%;
    width: 200px;
    position: fixed;
    z-index: 1;
    top: 0;
    left: 0;
    background-color: #111;
    overflow-x: hidden;
}

/* Side navigation links */
.sidenav a {
    color: white;
    padding: 16px;
    text-decoration: none;
    display: block;
}

/* Change color on hover */
.sidenav a:hover {
    background-color: #ddd;
    color: black;
}

/* Style the content */
.content {
    margin-left: 200px;
    padding-left: 20px;
}

img,
video {
    max-width: 50%;
    height: auto;
}
</style>