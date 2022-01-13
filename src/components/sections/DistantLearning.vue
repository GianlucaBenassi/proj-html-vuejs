<template>
    <section>
        <div class="container py-5">

            <!-- title row -->
            <div class="row row-cols-1 row-cols-md-2 align-items-center mb-5">

                <!-- title -->
                <div class="col mb-5 mb-md-0 title" :class="{'text-center' : dataShared.smScreen}">
                    <h1 class="big-title">Distant learning for further expansion</h1>
                    <p class="mt-2 text-color-light">Learning is a life-long journey that in fact we find the terminate stop. Stop searching, enjoy the process.</p>
                    <button class="mt-5 mb-4 btn-green"><i class="fas fa-download"></i> Download free guide</button>
                    <a href="#" class="d-block text-color-light">
                        Have questions? 
                        <span class="text-green">Get Free Sample <i class="fas fa-long-arrow-alt-right"></i></span>
                    </a>
                </div>

                <!-- image -->
                <div class="col me-image">
                    <img src="../../assets/img/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg" alt="about me image" class="coach">
                    <img src="../../assets/img/maxcoach-shape-08.png" alt="shape 01" class="shape sh-01 d-none d-md-block">
                    <img src="../../assets/img/maxcoach-shape-07.png" alt="shape 02" class="shape sh-02 d-none d-md-block">
                    <img src="../../assets/img/maxcoach-shape-02.png" alt="shape 03" class="shape sh-03">
                    <div class="shape circle-shape koromiko"></div>
                </div>

            </div>

            <!-- logos row -->
            <div class="row row-cols-2 row-cols-md-3 row-cols-lg-6 align-items-center row-bottom">
                
                <div class="col d-flex justify-content-center mb-3 mb-lg-0">
                    <img src="../../assets/img/client-logo-01.png" alt="stylus logo">
                </div>
                
                <div class="col d-flex justify-content-center mb-3 mb-lg-0">
                    <img src="../../assets/img/client-logo-02.png" alt="coffe tree logo">
                </div>
                
                <div class="col d-flex justify-content-center mb-3 mb-lg-0">
                    <img src="../../assets/img/client-logo-03.png" alt="brook logo">
                </div>
                
                <div class="col d-flex justify-content-center mb-3 mb-lg-0">
                    <img src="../../assets/img/client-logo-04.png" alt="pencil logo">
                </div>
                
                <div class="col d-flex justify-content-center mb-3 mb-lg-0">
                    <img src="../../assets/img/client-logo-05.png" alt="its alive! logo">
                </div>
                
                <div class="col d-flex justify-content-center mb-3 mb-lg-0">
                    <img src="../../assets/img/client-logo-06.png" alt="sixbase logo">
                </div>

            </div>

        </div>
    </section>
</template>

<script>
import dataShared from '../../shared/dataShared';

export default {
    name: 'DistantLearning',
    data() {
        return {
            dataShared
        }
    }
}
</script>

<style lang='scss' scoped>

.title a span {
    font-weight: bold;
}

.me-image {
    position: relative;
    
    .coach {
        width: 100%;
        border-radius: 50%;
    }

    .shape {
        position: absolute;

        &.sh-01 {
            top: 40%;
            left: -30px;
            z-index: -1;
        }

        &.sh-02 {
            bottom: 10px;
            right: 20%;
            z-index: -1;
        }

        &.sh-03 {
            top: 20%;
            right: 20px;
            z-index: 1;
        }

        &.circle-shape {
            bottom: 20%;
            left: 0;
        }
    }
}

.row-bottom img {
    opacity: 50%;
    transition: all .3s;
    
    &:hover {
        opacity: 100%;
    }
}

</style>