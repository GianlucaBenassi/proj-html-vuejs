<template>
    <section>

        <!-- wave -->
        <svg class="d-block" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#f6f3f5" fill-opacity="1" d="M0,224L120,229.3C240,235,480,245,720,208C960,171,1200,85,1320,42.7L1440,0L1440,320L1320,320C1200,320,960,320,720,320C480,320,240,320,120,320L0,320Z"></path></svg>

        <div class="container-fluid section-bg-grey pb-5">
            
            <!-- title -->
            <h3 class="sub-title text-center">Great words about maxcoach</h3>
            <h2 class="mt-2 mb-5 medium-title text-center">Our <span class="text-green">top learners'</span> verbatim</h2>

            <!-- carousel -->
            <CustomSwiper/>

            <!-- get start now -->
            <div class="get_start text-center mb-5">
                <h3 class="mt-5">Start today for getting <span class="text-green">Online Certification</span></h3>
                <h2 class="mt-2 mb-5 big-title">You can be your own guiding star with our help!</h2>
                <button class="btn-green">Get started now</button>

                <img src="../../assets/img/maxcoach-shape-01.png" alt="shape 01" class="shape sh-01">
                <img src="../../assets/img/maxcoach-shape-02.png" alt="shape 02" class="shape sh-02">
                <div class="circle-shape koromiko shape"></div>
            </div>

        </div>

    </section>
</template>

<script>
import CustomSwiper from '../commons/CustomSwiper.vue';

export default {
    name: 'TopLearners',
    components: {
        CustomSwiper
    }
}
</script>

<style lang='scss' scoped>

h2 span,
h3 span {
    font-weight: normal;
}

.get_start {
    position: relative;

    .shape {
        position: absolute;

        &.sh-01 {
            top: 50%;
            left: 20%;
        }

        &.sh-02 {
            top: 60%;
            right: 10%;
        }

        &.circle-shape {
            top: 15%;
            left: 18%;
        }
    }
}

</style>