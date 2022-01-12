<template>
    <section>
        <div class="container pt-5">

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

            <!-- YouTube video -->
            <div class="row yt_video">

                <!-- video -->
                <div class="col-7">
                    <a href="#" class="d-block youtube">
                        <div class="video">
                            <img src="../../assets/img/home-2-popup-video-poster.jpg" alt="Companionship video" class="d-block">
                        </div>
                        <img src="../../assets/img/icon-youtube-play.png" alt="YouTube logo" class="yt_logo">
                        <img src="../../assets/img/maxcoach-shape-05.png" alt="shape-01" class="shape sh-01">
                        <img src="../../assets/img/maxcoach-shape-09.png" alt="shape-02" class="shape sh-02">
                        <img src="../../assets/img/maxcoach-shape-07.png" alt="shape-03" class="shape sh-03">
                        <div class="shape circle-shape koromiko"></div>
                    </a>
                </div>

                <!-- description -->
                <div class="col-5 mt-5 ps-5">
                    <h3 class="sub-title">get started <span class="text-color">effortlessly</span></h3>
                    <h2 class="mt-3 mb-4 big-title">Enjoy Our <span class="text-green">companionship</span></h2>
                    <p class="text-color-light mb-5">Sneek peek into what jas in store for you on our online traching and mentoring portal. Seek for some hidden hint of early-bird rewards as well.</p>
                    <a href="#" class="text-green">Download guidebook <i class="fas fa-long-arrow-alt-right"></i></a>
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
    margin-bottom: 170px;

    .fa-long-arrow-alt-right {
        margin-left: 6px;
    }
}


.yt_video {

    .youtube {
        border-radius: 5px;
        position: relative;


        .video {
            border-radius: inherit;
            overflow: hidden;
            img {
                width: 100%;
                transition: all .8s;
            }
        }

        &:hover .video img {
            transform: scale(1.1);
        }

        .yt_logo {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            z-index: 1;
        }

        .shape {
            position: absolute;
            z-index: -1;

            &.sh-01 {
                top: 50px;
                left: -60px;
            }

            &.sh-02 {
                top: -100px;
                left: -40px;
            }

            &.sh-03 {
                bottom: -100px;
                right: -15px;
            }

            &.circle-shape {
                top: -40px;
                right: -80px;
            }
        }
    }

}

</style>