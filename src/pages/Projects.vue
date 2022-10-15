<template>
    <div>
        <Navbar />
        <section class="faverite">
            <h1 class="heading"> <span>my</span> Trailer Movies </h1>
            <h3>ผ้าผีบอก | Official Trailer </h3>
            <p>ระเบิดความฮา ไขปมปริศนา
                    #ผ้าผีบอก 23 มิถุนายนนี้ ทุกโรงภาพยนตร์
                    
                    #BNK48หมกกบ_MV 
                    
                    #ผ้าผีบอก23มิถุนายนนี้ 
                    #BNK48 #หยิ่นวอร์  </p>
            <div class="box-container">
                <center><iframe width="560" height="315" src="https://www.youtube.com/embed/0YAvS9eWnRk"
                        title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; 
                    gyroscope; picture-in-picture" allowfullscreen>
                     </iframe> </center>
            </div>
        </section>
    </div>
</template>

<script>
import Navbar from '../components/Navbar.vue';
export default {
    components: { Navbar }
}
</script>

<style>

</style>