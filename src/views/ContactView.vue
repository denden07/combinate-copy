<template>
    <Banner :title="title" :details="details" :show="show"/>
    <Form/>
</template>

<script>
    import Banner from '../components/Banner.vue'
    import Form from '../components/Contact/Form.vue'
    export default {
        components: {
            Banner,
            Form
        },
        data() {
            return {
                title: 'Get in Touch',
                details: "Let’s make something awesome together. Drop us a line, and we'll be in touch as soon as possible.",
                show: false
            }
        }
    }
</script>