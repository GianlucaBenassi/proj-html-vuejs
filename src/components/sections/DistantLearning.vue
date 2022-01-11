<template>
    <section>
        <div class="container">

            <!-- title row -->
            <div class="row row-top">

                <!-- title -->
                <div class="col title">
                    <h1 class="big-title">Distant learning for further expansion</h1>
                    <p class="text-color-light">Learning is a life-long journey that in fact we find the terminate stop. Stop searching, enjoy the process.</p>
                    <button class="btn-green"><i class="fas fa-download"></i> Download free guide</button>
                    <a href="#" class="text-color-light">
                        Have questions? 
                        <span class="text-green">Get Free Sample <i class="fas fa-long-arrow-alt-right"></i></span>
                    </a>
                </div>

                <!-- image -->
                <div class="col me-image">
                    <img src="../../assets/img/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg" alt="about me image" class="coach">
                    <img src="../../assets/img/maxcoach-shape-08.png" alt="shape 01" class="shape sh-01">
                    <img src="../../assets/img/maxcoach-shape-07.png" alt="shape 02" class="shape sh-02">
                    <img src="../../assets/img/maxcoach-shape-02.png" alt="shape 03" class="shape sh-03">
                    <div class="shape circle-shape koromiko"></div>
                </div>

            </div>

            <!-- logos row -->
            <div class="row row-bottom">
                
                <div class="col">
                    <img src="../../assets/img/client-logo-01.png" alt="stylus logo">
                </div>
                
                <div class="col">
                    <img src="../../assets/img/client-logo-02.png" alt="coffe tree logo">
                </div>
                
                <div class="col">
                    <img src="../../assets/img/client-logo-03.png" alt="brook logo">
                </div>
                
                <div class="col">
                    <img src="../../assets/img/client-logo-04.png" alt="pencil logo">
                </div>
                
                <div class="col">
                    <img src="../../assets/img/client-logo-05.png" alt="its alive! logo">
                </div>
                
                <div class="col">
                    <img src="../../assets/img/client-logo-06.png" alt="sixbase logo">
                </div>

            </div>

        </div>
    </section>
</template>

<script>
export default {
    name: 'DistantLearning'
}
</script>

<style lang='scss' scoped>

.container {
    padding: 50px 0;
}

.row {
    align-items: center;

    &.row-top {
        margin-bottom: 60px;
    }
}

.title {

    p {
        margin-top: 10px;
    }

    button {
        margin: 40px 0 20px 0;
    }

    a {
        display: block;

        span {
            font-weight: bold;
        }
    }
}

.me-image {
    position: relative;
    
    .coach {
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
            right: -20px;
            z-index: 1;
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