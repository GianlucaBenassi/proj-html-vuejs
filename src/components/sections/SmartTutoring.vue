<template>
    <section>
        <div class="container py-5">

            <!-- title -->
            <h3 class="sub-title text-center">maxcoach available courses</h3>
            <h2 class="mt-2 mb-5 medium-title text-center">Access <span class="text-green">Smart Tutoring</span> Program For Benefits.</h2>

            <!-- info cards -->
            <div class="row info_cards">

                <div class="col">
                    <img src="../../assets/img/home-2-image-box-01.png" alt="Preferences image">
                    <h3 class="my-3">Customize Preferences</h3>
                    <p class="text-color-light mb-3">Learners are given the right to arrange and customize their study schedule and timetable based on preferences.</p>
                    <a href="#" class="text-gunPowder hover-text-green">Start here <i class="fas fa-long-arrow-alt-right"></i></a>
                </div>

                <div class="col">
                    <img src="../../assets/img/about-us-02-image-box-02.png" alt="Preferences image">
                    <h3 class="my-3">Cloud Storage</h3>
                    <p class="text-color-light mb-3">You can store lessons via online cloud or download to your device and revise lessons on the way.</p>
                    <a href="#" class="text-gunPowder hover-text-green">Get Free Quote <i class="fas fa-long-arrow-alt-right"></i></a>
                </div>

                <div class="col">
                    <img src="../../assets/img/home-2-image-box-03.png" alt="Preferences image">
                    <h3 class="my-3">Multimedia Channels</h3>
                    <p class="text-color-light mb-3">We provide study materials with various formats: video, audio, slide, doc, prints, books and applications.</p>
                    <a href="#" class="text-gunPowder hover-text-green">Start now <i class="fas fa-long-arrow-alt-right"></i></a>
                </div>

            </div>

        </div>
    </section>
</template>

<script>
export default {
    name: 'SmartTutoring'
}
</script>

<style lang='scss' scoped>

h2 span{
    font-weight: normal;
}

.info_cards {
    .fa-long-arrow-alt-right {
        margin-left: 6px;
    }
}

</style>