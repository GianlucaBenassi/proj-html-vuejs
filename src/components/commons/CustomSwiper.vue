<template>
    <swiper ref="mySwiper" :options="swiperOptions">

        <swiper-slide class="sw_slide p-5">
            <h3>High level of efficiency and scientific teaching methods</h3>
            <p class="text-color-light mt-3 mb-5">I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.</p>
            <div class="user d-flex">
                <img src="../../assets/img/testimonial-avata-02.jpg" alt="Mina Hollance">
                <div class="ms-3">
                    <span class="d-block mt-2 name">Mina Hollance</span>
                    <span class="d-block mt-3 text-color-light">/ Freelancer</span>
                </div>
            </div>
        </swiper-slide>

        <swiper-slide class="sw_slide p-5">
            <h3>Professional team of specialists and passionate mentors at reach</h3>
            <p class="text-color-light mt-3 mb-5">I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.</p>
            <div class="user d-flex">
                <img src="../../assets/img/testimonial-avata-04.jpg" alt="Madley Pondor">
                <div class="ms-3">
                    <span class="d-block mt-2 name">Madley Pondor</span>
                    <span class="d-block mt-3 text-color-light">/ IT Specialist</span>
                </div>
            </div>
        </swiper-slide>

        <swiper-slide class="sw_slide p-5">
            <h3>The MaxCoach team works really hard to ensure high quality</h3>
            <p class="text-color-light mt-3 mb-5">I am happy with their arrangement of lessons and subjects. They reflect a scintific investigation into effective methods to be adopted for learners of all levels.</p>
            <div class="user d-flex">
                <img src="../../assets/img/testimonial-avata-01.jpg" alt="Luvic Dubble">
                <div class="ms-3">
                    <span class="d-block mt-2 name">Luvic Dubble</span>
                    <span class="d-block mt-3 text-color-light">/ Private Tutor</span>
                </div>
            </div>
        </swiper-slide>

        <swiper-slide class="sw_slide p-5">
            <h3>It's a chiuce of quality for people with special needs</h3>
            <p class="text-color-light mt-3 mb-5">I'm a very strict person so I require everything to be organized and neat. Then, I'll be able to make things right and shine. MaxCoach guys just got me.</p>
            <div class="user d-flex">
                <img src="../../assets/img/testimonial-avata-03.jpg" alt="Florence Themes">
                <div class="ms-3">
                    <span class="d-block mt-2 name">Florence Themes</span>
                    <span class="d-block mt-3 text-color-light">/ Multimedia Admin</span>
                </div>
            </div>
        </swiper-slide>

        <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
</template>

<script>
import {Swiper, SwiperSlide, directive} from 'vue-awesome-swiper';
import 'swiper/css/swiper.css';

export default {
    name: 'CustomSwiper',
    components: {
        Swiper,
        SwiperSlide
    },
    directives: {
        swiper: directive
    },
    data() {
        return {
            swiperOptions: {
                slidesPerView: 3,
                spaceBetween: 30,
                loop: true,
                centeredSlides: true,
                pagination: {
                    clickable: true,
                    el: '.swiper-pagination'
                }
            }
        }
    },
    computed: {
        swiper() {
            return this.$refs.mySwiper.$swiper;
        }
    }
}
</script>

<style lang='scss'>

@import '../../assets/style/_variables.scss';

.sw_slide {
    background-color: #fff;
    height: auto;
    border-radius: 5px;

    .user {
        img {
            border-radius: 50%;
            height: 70px;
        }
        .name {
            color: $gunPowder;
            font-weight: bold;
            text-transform: uppercase;
        }
    }
}

.swiper-pagination {
    position: relative;

    &.swiper-pagination-bullets{
        bottom: 0;
        margin-top: 30px;
    }
}

.swiper-pagination-bullet {
    margin: 0 10px !important;
    transition: all .3s;

    &:hover {
        background-color: $gunPowder;
        transform: scale(1.5);
        opacity: 1;
    }
}

.swiper-pagination-bullet-active {
    background-color: $gunPowder;
    transform: scale(1.5);
}

</style>