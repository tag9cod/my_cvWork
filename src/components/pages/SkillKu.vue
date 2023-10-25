<template>
    <section class="py-5 border-bottom wow fadeInUp" data-wow-delay="0.1s">
        <h2 class="title pb-3 mb-5 text-primary mt-2">Skills</h2>
        <div class="row">
            <div class="col-sm-6">
                <div class="col-12 text-center mb-2"><div class="service-item" style="border-top-left-radius:10px ;"><h6>Hard Skill</h6></div></div>
                <div class="service-item" style="border-bottom-left-radius: 10px;">
                    <div class="skill mb-4" v-for="hard, index in skillHard" :key="index">
                        <div class="d-flex justify-content-between">
                            <p class="mb-2">{{ hard.name }}</p>
                            <p class="mb-2">{{ hard.level }}</p>
                        </div>
                        <div class="progress">
                            <div class="progress-bar bg-primary" role="progressbar" aria-valuemin="0" aria-valuemax="100"></div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-sm-6">
                <div class="col-12 text-center mb-2"><div class="service-item" style="border-top-right-radius:10px;"><h6>Soft Skill</h6></div></div>
                <div class="service-item" style="border-bottom-right-radius: 10px;">
                    <div class="skill mb-4" v-for="soft, index in skillSoft" :key="index">
                        <div class="d-flex justify-content-between">
                            <p class="mb-2">{{ soft.name }}</p>
                            <p class="mb-2">{{ soft.level }}</p>
                        </div>
                        <div class="progress">
                            <div class="progress-bar bg-danger" role="progressbar" aria-valuenow="90" aria-valuemin="0" aria-valuemax="90"></div>
                        </div>
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
                skillHard: [
                    {name: "Vue js", level: "Basic"}, 
                    {name: "Laravel", level: "Basic"},
                    {name: "PHP", level: "Basic"},
                    {name: "Bootstrap", level: ""},
                    {name: "MySql", level: ""},
                    {name: "Git Control", level: ""},
                    {name: "Postman", level: ""},
                    {name: "Tiktok Ads", level: ""},
                    {name: "Ubbersuggest", level: ""},
                    {name: "Semrush", level: ""},
                    {name: "Ms. Office", level: ""},
                ],
                skillSoft: [
                    {name: "Interpersonal Skill", level: ""}, 
                    {name: "Communication", level: ""},
                    {name: "Fast Learner", level: ""},
                    {name: "Responsibility", level: ""},
                    {name: "Adaptable", level: ""},
                    {name: "Team Work", level: ""},
                    {name: "Leadership", level: ""},
                    {name: "Negotiation", level: ""},
                    {name: "Problem Solving", level: ""},
                    {name: "Critical Thinking", level: ""},
                    {name: "Administrative Servant", level: ""},
                ],
            };
        },
    };
</script>