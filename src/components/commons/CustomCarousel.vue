<template>
    <carousel 
        :per-page="3" 
        :mouse-drag="true"
        :scrollPerPage="true"
        :loop="true"
    >
        <slide>
            Slide 1 Content
        </slide>
        <slide>
            Slide 2 Content
        </slide>
        <slide>
            Slide 3 Content
        </slide>
        <slide>
            Slide 4 Content
        </slide>
    </carousel>
</template>

<script>
import { Carousel, Slide } from 'vue-carousel';

export default {
    name: 'CustomCarousel',
    components: {
        Carousel,
        Slide
    }
}
</script>

<style lang='scss' scoped>

</style>