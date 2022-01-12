<template>
    <swiper ref="mySwiper" :options="swiperOptions">
        <swiper-slide class="sw_slide">Slide 1</swiper-slide>
        <swiper-slide class="sw_slide">Slide 2</swiper-slide>
        <swiper-slide class="sw_slide">Slide 3</swiper-slide>
        <swiper-slide class="sw_slide">Slide 4</swiper-slide>
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
                slidePrevClass: 'swiper-slide-prev sw_prev',
                slideNextClass: 'swiper-slide-next sw_next',
                pagination: {
                    clickable: true,
                    el: '.swiper-pagination'
                }
            }
        }
    },
    computed: {
        swiper() {
            return this.$refs.mySwiper.$swiper
        }
    }
}
</script>

<style lang='scss'>

.sw_slide {
    background-color: red;
    height: 200px;
}

</style>