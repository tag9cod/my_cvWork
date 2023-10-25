<template>
    <about/>
    <pengalaman/>
    <sikil/>
    <pelatihan/>
    <forto/>
</template>

<script>
import about from '../components/pages/AboutMe.vue'
import sikil from '../components/pages/SkillKu.vue'
import pengalaman from '../components/pages/KerjaKu.vue'
import pelatihan from '../components/pages/SertifikasiKu.vue'
import forto from '../components/pages/FortoPolioku.vue'
    export default {
        name: 'mainBar',
        components:{
            about,
            sikil,
            pengalaman,
            pelatihan,
            forto
        }
    }
</script>