<template>
    <div class="sub-container">
        <header class="header">
            <h1>Skills</h1>
        </header>
        <div class="expertise">
            <div class="skill" v-for="exp in expertise" :key="exp.id">
                <p>{{ exp.language }} <span>{{ exp.level }}</span> </p>
                <div class="progress-bar">
                    <div class="progress-fill" :style="{'width': exp.level}"></div>
                </div>
            </div>
        </div>
        <div class="skills" v-if="skillsDisplay">
            <div class="skill" v-for="skill in skills" :key="skill.id">
                <p>{{ skill.language }} <span>{{ skill.level }}</span> </p>
                <div class="progress-bar">
                    <div class="progress-fill" :style="{'width': skill.level}"></div>
                </div>
            </div>
        </div>
        <button class="show-additional-skills" @click="skillsDisplay = !skillsDisplay">
            <span v-if="!skillsDisplay">Show More</span>
            <span v-else>Show Less</span>  
            <!-- <span :class="{ active: skillsDisplay }"><i class="medium material-icons">expand_more</i></span>   -->
            <span v-if="!skillsDisplay"><i class="fas fa-expand-arrows-alt"></i></span>
            <span v-else><i class="fas fa-compress-arrows-alt"></i></span>
        </button>
    </div>
</template>

<script>
export default {
    name: "Skills",
    data(){
        return {
            expertise: [
                {
                    id: 1,
                    language: "HTML 5",
                    level: "85%",
                },
                {
                    id: 2,
                    language: "CSS 3",
                    level: "80%"
                },
                {
                    id: 3,
                    language: "JavaScript",
                    level: "80%"
                },
                {
                    id: 4,
                    language: "Vue JS",
                    level: "75%"
                },
                {
                    id: 5,
                    language: "Laravel",
                    level: "70%"
                }
            ],
            skills: [
                {
                    id: 1,
                    language: "C#",
                    level: "40%"
                },
                {
                    id: 2,
                    language: "ASP.NET Core",
                    level: "35%"
                },
                {
                    id: 3,
                    language: "PHP",
                    level: "60%",
                },
                {
                    id: 4,
                    language: "MySql",
                    level: "50%"
                },
                {
                    id: 5,
                    language: "Firebase",
                    level: "65%"
                },
                {
                    id: 6,
                    language: "React JS",
                    level: "30%"
                },
                {
                    id: 7,
                    language: "React Native",
                    level: "20%"
                },
                {
                    id: 8,
                    language: "Python",
                    level: "40%"
                },
                {
                    id: 9,
                    language: "GIT",
                    level: "60%"
                },
                {
                    id: 10,
                    language: "Unity Game Development",
                    level: "30%",
                },
                {
                    id: 11,
                    language: "SEO",
                    level: "40%"
                },
                {
                    id: 12,
                    language: "Responsive Web Design",
                    level: "70%"
                },
                { id: 13, language: "Photoshop", level: "30%" }
            ],
            skillsDisplay: false
        }
    }
}
</script>

<style>

</style>
