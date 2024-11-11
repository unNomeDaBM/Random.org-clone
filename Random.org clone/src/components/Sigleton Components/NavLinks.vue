<template>
    <nav>
        <NavLink v-for="linkName, idx of linksNames" id="idx">
            {{ linkName }}
        </NavLink>
    </nav>
</template>

<script>
import NavLink from '../Reusable Components/NavLink.vue';

    export default{
        data(){
            return{
                linksNames: ["Home", "Games", "Numbers", "Lists & More", "Drawings", "Web Tools", "Statistics", "Testimonials", "Learn More", "Login"],

            }
        },
        components:{NavLink}
    }
</script>

<style scoped>
    nav{
        padding: 10px 24px;

        display: flex;
        gap: 26px;
    }
</style>