<template>
    <section class="py-5 border-bottom wow fadeInUp" data-wow-delay="0.1s">
        <h2 class="title pb-3 mb-5 text-primary mt-2">About Me</h2>
        <p align="justify">
            Saya lulusan sistem informasi yang siap bekerja dibidang apapun dengan bekal pengalaman kerja sebagai Admin Internal Audit ( Magang Offline),
            Staff Produksi, Digital Marketing Specialist ( Magang Online ), Fullstack Developer ( Magang Online ) dan SEO Outreach ( Magang Online ).
        </p>
        <div class="row mb-4" v-for="status, index in tentang" :key="index">
            <div class="col-sm-6 py-1">
                <span class="fw-medium text-primary">Universitas:</span> {{ status.kuliah }}
            </div>
            <div class="col-sm-6 py-1">
                <span class="fw-medium text-primary">Email          :</span> {{ status.imel }}
            </div>
            <div class="col-sm-6 py-1">
                <span class="fw-medium text-primary">Jurusan    :</span> {{ status.jurusan }}
            </div>
            <div class="col-sm-6 py-1">
                <span class="fw-medium text-primary">Phone          :</span> {{ status.phone }}
            </div>
            <div class="col-sm-6 py-1">
                <span class="fw-medium text-primary">IPK        :</span> {{ status.ipk }}
            </div>
            <div class="col-sm-6 py-1">
                <span class="fw-medium text-primary">Tanggal Lahir  :</span> {{ status.lahir }}
            </div>
            <div class="col-sm-6 py-1">
                <span class="fw-medium text-primary">Tahun      :</span> {{ status.tahun }}
            </div>
            <div class="col-sm-6 py-1">
                <span class="fw-medium text-primary">Address        :</span> {{ status.alamat }}
            </div>
        </div>
        <div class="row g-4">
            <div class="col-md-4 col-lg-6 col-xl-4" v-for="ringkas, index in ringkasan" :key="index">
                <div class="d-flex bg-secondary p-4" style="border-radius:5px">
                    <h1 class="flex-shrink-0 display-5 text-primary mb-0" data-toggle="counter-up">{{ ringkas.jml }}</h1>
                    <div class="ps-3">
                        <p class="mb-0">{{ ringkas.ttl }}</p>
                        <h6 class="mb-0">{{ ringkas.name }}</h6>
                    </div>
                </div>
            </div>
           
        </div>
    </section>
</template>

<script>
    export default {
        data() {
            return {
                tentang: [
                    {
                        imel: "tgunawant@gmail.com",
                        phone: "081905072949",
                        lahir: "09 Mei 1990",
                        alamat: "Permata Balaraja, Tangerang - Banten",
                        kuliah: "STMIK Insan Pembangunan",
                        jurusan: "Sistem Informasi",
                        ipk: "3.19",
                        tahun: "2015 - 2019"
                    },
                ],
                ringkasan: [
                    {jml: "2", ttl: "Total", name: "Pengalaman Kerja"},
                    {jml: "4", ttl: "Total", name: "Project Based"},
                    {jml: "4", ttl: "Total", name: "Course"},
                ]
            };
        },
    };
</script>