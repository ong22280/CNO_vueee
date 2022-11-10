<template>

    <div class="text-center text-white text-5xl font-bold p-12">
        <button @click="dropdown=!dropdown">menu</button>
        <div class="animate-fadeIn" v-if="dropdown">
            this is dropdown
        </div>

        <dir>
            this is on change
        </dir>
        <input class="text-black" type="text" @change="count++">
        <div>
            count is {{count}}
        </div>
        
        <div>this is v-model</div>
        <input class="text-black" type="text" v-model="name">
        <p>{{name}}</p>

        <font-awesome-icon icon="fa-regular fa-house" />
    </div>
</template>

<script>
export default {
    data() {
        return {
            count: 0,
            dropdown: false,
            name: "ong"
        }
    }
}
</script>

<style>

</style>