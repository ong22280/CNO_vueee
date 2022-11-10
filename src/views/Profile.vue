<template >
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

    <div class="content text-white font-bold">
        <h1 class="text-4xl p-3">CNO Team</h1>


        <div v-for="member in members" :key="member.id" :member="member">
            <profile-card v-if="member.isMember"
                :imagePro="member.imagePro" 
                :name="member.name" 
                :studentID="member.studentID" 
                :college="member.college"
                :instagram="member.instagram"
                :image="member.image"
                :link="member.link"
            ></profile-card>
        </div>


        <div>
            <profile-card></profile-card>
            <profile-card></profile-card>
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
            image: "https://scontent.fbkk10-1.fna.fbcdn.net/v/t39.30808-6/295730370_3367991310154632_3425117977811074482_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=09cbfe&_nc_eui2=AeHYKq3vAUNsStHqOWYDrua9BtlgHfNT9YYG2WAd81P1hu4KAB7msDtuMaBMzYbx6OgZSxQI2mvCzmatD54r8B_6&_nc_ohc=ENW_q_11CNIAX-4nWfb&_nc_ht=scontent.fbkk10-1.fna&oh=00_AfCt_7SGIXcRb5xiN_mv8t7KslqUarCv5YhfsJevj5RBUA&oe=637108E8",
            link: "https://www.instagram.com/sittipongong/"
        }
    },
    components: {
        profileCard
    },
    data() {
        return {
            members: [
                {
                    imagePro: '../assets/images/ong.png',
                    name: "Sittipong Hemloun",
                    studentID: "6410401183",
                    college: "Kasetsart University",
                    instagram: "sittipongong",
                    image: "https://scontent.fbkk10-1.fna.fbcdn.net/v/t39.30808-6/295730370_3367991310154632_3425117977811074482_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=09cbfe&_nc_eui2=AeHYKq3vAUNsStHqOWYDrua9BtlgHfNT9YYG2WAd81P1hu4KAB7msDtuMaBMzYbx6OgZSxQI2mvCzmatD54r8B_6&_nc_ohc=ENW_q_11CNIAX-4nWfb&_nc_ht=scontent.fbkk10-1.fna&oh=00_AfCt_7SGIXcRb5xiN_mv8t7KslqUarCv5YhfsJevj5RBUA&oe=637108E8",
                    link: "https://www.instagram.com/sittipongong/",
                    isMember: true
                },
                {
                    imagePro: '../assets/images/ong.png',
                    name: "Punnatud Duengkae",
                    studentID: "6410406771",
                    college: "Kasetsart University",
                    instagram: "nokkokalderaan",
                    image: "https://scontent.fbkk10-1.fna.fbcdn.net/v/t31.18172-8/26233019_2018331688407504_7732129327440678024_o.jpg?_nc_cat=107&ccb=1-7&_nc_sid=09cbfe&_nc_eui2=AeEjFHeqVxvYoY3RKaETB_99GTGK65gdfIYZMYrrmB18hjSPnGXlY9AmC64rfBBMneMGBwkgIbcinRiXPFUVPfnK&_nc_ohc=mB1czETJBEsAX-vQO4v&tn=HcEiJXWqLH7xYntm&_nc_ht=scontent.fbkk10-1.fna&oh=00_AfD2ysbnuXLwktjUTCJ4W6kttfG-3XlqgnREcPttzjeG6g&oe=6393D177",
                    link: "https://www.instagram.com/nokkokalderaan/",
                    isMember: true
                },
                {
                    imagePro: '../assets/images/ong.png',
                    name: "Patinya Saichantadee",
                    studentID: "6410406754",
                    college: "Kasetsart University",
                    instagram: "cxld.pty",
                    image: "https://scontent.fbkk10-1.fna.fbcdn.net/v/t39.30808-6/306148111_1880034558867492_7239761071913403261_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=09cbfe&_nc_eui2=AeH1gcHXA61bXexlWxN3EKag3vZh_X94_pHe9mH9f3j-kekdG3NFekUESEaVMeskPsQzsd5OaXwhpb5dwuIlJESs&_nc_ohc=X2MKA-ZW1JcAX-HU3kp&_nc_ht=scontent.fbkk10-1.fna&oh=00_AfAxTEUvhsOUfYVKlh1U6hZY9EXCCuCuFyaT5jttCR3q8A&oe=63706736",
                    link: "https://www.instagram.com/cxld.pty/",
                    isMember: true
        
                },
                {
                    imagePro: '../assets/images/ong.png',
                    name: "Patinya Saichantadee",
                    studentID: "6410406754",
                    college: "Kasetsart University",
                    instagram: "cxld.pty",
                    image: "https://scontent.fbkk10-1.fna.fbcdn.net/v/t39.30808-6/306148111_1880034558867492_7239761071913403261_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=09cbfe&_nc_eui2=AeH1gcHXA61bXexlWxN3EKag3vZh_X94_pHe9mH9f3j-kekdG3NFekUESEaVMeskPsQzsd5OaXwhpb5dwuIlJESs&_nc_ohc=X2MKA-ZW1JcAX-HU3kp&_nc_ht=scontent.fbkk10-1.fna&oh=00_AfAxTEUvhsOUfYVKlh1U6hZY9EXCCuCuFyaT5jttCR3q8A&oe=63706736",
                    link: "https://www.instagram.com/cxld.pty/",
                    isMember: false
        
                },
            ]
        }
    }
};
</script>
