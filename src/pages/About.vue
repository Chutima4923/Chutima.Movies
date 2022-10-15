<template>
    <div>
        <Navbar />

        <section class="about">

            <h1 class="heading"> About <span>Movies</span> </h1>

            <div class="row">

                <div class="info-container">

                    <div class="info-container">

                     <h1>ผู้กำกับ: ณัฐพงษ์ อรุณเนตร์</h1>
                     <h1>นำแสดงโดย: วีรยา จาง, มิลิน ดอกเทียน, วนรัตน์ รัศมีรัตน์</h1>
                     <h1>ความยาว: 96 นาที</h1>
                     <h1>กำหนดฉายในไทย: 23 มิถุนายน 2022 (ในโรงภาพยนตร์)</h1>

                    </div>

                </div>

                <div class="count-container">

                    <div class="box">
                        <h3>6/10</h3>
                        <p>ภาพรวม</p>
                    </div>

                    <div class="box">
                        <h3>5/10</h3>
                        <p>เล่าเรื่อง</p>
                    </div>

                    <div class="box">
                        <h3>7/10</h3>
                        <p>การแสดง</p>
                    </div>

                    <div class="box">
                        <h3>7/10</h3>
                        <p>เทคนิคงานสร้าง</p>
                    </div>

                    <div class="box">
                        <h3>5/10</h3>
                        <p>บทภาพยนตร์</p>
                    </div>

                </div>

            </div>

        </section>

        <!-- about section ends -->

 
        <!-- education section starts  -->

        <section class="education">

            <h1 class="heading"> <span>my</span> experience </h1>

            <div class="box-container">

                <div class="box">
                    <i class="fas fa-briefcase"></i>
                    <span>2020 - 2021</span>
                    <h3>uTech Solutions</h3>
                    <p>Assist the system analyst in conduct analysis, architecture, design database model for the new
                        application.</p>
                </div>

            </div>

        </section>
    </div>
</template>

<script>
import Navbar from "../components/Navbar.vue";
import axios from 'axios' 
export default {
    components: { Navbar },
    methods: {
        async felchExprience() {
            try {
                let res = await axios.get("https://633fc566e44b83bc73c0f545.mockapi.io/profile/v1/experiences")
                this.experiences + res.data
            } catch (error) {

            }
        }
    },
    data() {
        return {
            experiences : []
        }
    },
    beforeMount() {
        this.felchExprience()
    }
}
</script>

<style>

</style>