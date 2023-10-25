<template>
    <section class="py-5 border-bottom wow fadeInUp" data-wow-delay="0.1s">
        <h2 class="title pb-3 mb-5 text-primary mt-2">Sertifikasi</h2>
        <div class="row g-4">
            <div class="col-md-6" v-for="latih, index in pelatihan" :key="index">
                <div class="service-item" style="border-radius:5px">
                    <i class="fa fa-2x fa-laptop-code mx-auto mb-4"></i>
                    <h6 class="mb-2">{{ latih.name }}</h6>
                    <p class="mb-0">{{ latih.tahun }}</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        data() {
            return {
                pelatihan: [
                    {name: "Data Scientist -  Skill Academy", tahun: "Course - 2022"},
                    {name: "Belajar Javascript - Dicoding", tahun: "Course - 2022"},
                    {name: "Belajar Dasar DevOps - Dicoding", tahun: "Course - 2022"},
                    {name: "Belajar Dasar AWS Cloud - Dicoding", tahun: "Course - 2023"}
                ],
            };
        },
    };
</script>