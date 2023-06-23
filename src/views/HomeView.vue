<template>
    <Banner :title="title" :details="details" :show="show"/>
    <Services/>
</template>

<script>
    import Banner from '../components/Banner.vue'
    import Services from '../components/Home/services.vue'
    export default {
        components: {
            Banner,
            Services
        },
        data() {
            return {
                title: 'Software Development, Engineering and Consulting',
                details: "Solve your technological challenges using our team of experts and specialists. We'll tackle your problems and provide a cost effective solution using our experience gained from over 200 completed software projects.",
                show: true
            }
        }
    }
</script>