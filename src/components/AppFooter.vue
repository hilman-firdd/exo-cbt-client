<template>
    <footer class="c-footer bg-white d-flex justify-content-between">
        <div>&copy; 2019 - {{ year }} <span>Extraordinary-CBT {{ version }}</span></div>
     </footer>
</template>
<script>
    export default {
        data() {
            return {
                version: process.env.VUE_APP_VERSION,
                year: ''
            }
        },
        created() {
            let d = new Date()
            this.year = d.getFullYear()
        }
    }
</script>
