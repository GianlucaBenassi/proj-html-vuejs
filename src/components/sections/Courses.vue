<template>
    <section class="section-bg-grey">
        <div class="container py-5">
            
            <h3 class="sub-title text-center">Stimulated to learn?</h3>
            <h2 class="mt-2 medium-title text-center">Featured Online Courses</h2>

            <div class="row">
                <div class="col-6">
                    <CourseCard/>
                </div>
            </div>

        </div>
    </section>
</template>

<script>
import CourseCard from '../commons/CourseCard.vue';

export default {
    name: 'Courses',
    components: {
        CourseCard
    }
}
</script>

<style lang='scss' scoped>


</style>