<template>
    <section class="py-5 wow fadeInUp" data-wow-delay="0.1s">
        <h2 class="title pb-3 mb-5 text-primary mt-2"> Work Expericence</h2>
        <div class="service-item mb-4" style="text-align: left; border-radius: 10px;">
            <div class="border-start border-2 border-light pt-2 ps-5">
                <div class="position-relative mb-4" v-for="kerja, index in work" :key="index">
                    <span class="bi bi-arrow-right fs-4 text-light position-absolute" style="top: -5px; left: -50px;"></span>
                    <h5 class="mb-1">{{ kerja.bagian }}</h5>
                    <p class="mb-2">{{ kerja.kantor }} | <small>{{ kerja.durasi }}</small></p>
                    <p>{{ kerja.detail }}</p>
                </div>
            </div>
        </div>
        <h2 class="title pb-3 mb-5 text-primary mt-2"> Project Based - Online</h2>
        <div class="service-item mb-4" style="text-align: left; border-radius: 10px;">
            <div class="border-start border-2 border-light pt-2 ps-5">
                <div class="position-relative mb-4" v-for="projek, index in based" :key="index">
                    <span class="bi bi-arrow-right fs-4 text-light position-absolute" style="top: -5px; left: -50px;"></span>
                    <h5 class="mb-1">{{ projek.bagian }}</h5>
                    <p class="mb-2">{{ projek.kantor }} | <small>{{ projek.durasi }}</small></p>
                    <p>{{ projek.detail }}</p>
                </div>
            </div>
        </div>
    </section>
    <div class="d-flex align-items-end justify-content-between border-top mb-4"></div>
</template>

<script>
    export default {
        data() {
            return {
                work: [
                    { 
                        bagian: "Admin Internal Audit", 
                        kantor: "PT Lippo Karawaci Tbk", 
                        durasi: "Agustus - Oktober 2023",
                        detail: "Melakukan rekap data, mengecek data manajemen asset dan membuat laporan manajemen asset"
                    },
                    {
                        bagian: "Staff Produksi", 
                        kantor: "PT Surya Toto Indonesia Tbk",
                        durasi: "Februari 2013 - Januari 2023", 
                        detail: "Membantu proses produksi, mencatat hasil produksi dan membuat laporan hasil produksi"
                    },
                ],
                based: [
                    {
                        bagian: "Front End Development",
                        kantor: "PT Sinergi Peta - Inosoft Bootcamp",
                        durasi: "Maret - Juni 2023",
                        detail: "Membuat website manajemen vendor dengan vue js dan laravel sebagai back end"
                    },
                    {
                        bagian: "Digital Marketing Specialist",
                        kantor: "PT Qwords Company International",
                        durasi: "Mei - Juni 2023",
                        detail: "Melakukan market plan dengan Fb Ads dan Google Ads, Melakukan riset keyword"
                    },
                    {
                        bagian: "Fullstack Developer",
                        kantor: "PT Qwords Company International",
                        durasi: "Februari - Maret 2023",
                        detail: "Membuat landing page situs qwords.com dengan bahasa pemrogramman laravel dan bootstrap"
                    },
                    {
                        bagian: "SEO Outreach",
                        kantor: "PT Niagahoster",
                        durasi: "Desember 2022 - Januari 2023",
                        detail: "Melakukan riset keyword, Audit SEO, Backlink dan Strategi SEO"
                    },
                ],
            };
        },
    };
</script>