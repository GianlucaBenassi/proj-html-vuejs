<template>
    <section class="section-bg-grey">
        <div class="container py-5">
            
            <h3 class="sub-title text-center">Stimulated to learn?</h3>
            <h2 class="mt-2 mb-5 medium-title text-center">Featured Online Courses</h2>

            <div class="row row-cols-2 g-5">
                <div class="col" v-for="(course, index) in courses" :key="index">
                    <CourseCard :courseInfo="course"/>
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
    },
    data() {
        return {
            courses: [
                {
                    title: 'Learning to Write as a Professional Author',
                    price: 40.00,
                    img: require('../../assets/img/course-02-480x298.jpg'),
                    lessons: 20,
                    students: 50
                },
                {
                    title: 'Customer-centric Info-Tech Strategies',
                    price: 'Free',
                    img: require('../../assets/img/stock-full-hd-03-480x298.jpg'),
                    lessons: 24,
                    students: 769
                },
                {
                    title: 'Open Programming Courses for Everyone: Python',
                    price: 19.00,
                    img: require('../../assets/img/stock-full-hd-04-480x298.jpg'),
                    lessons: 17,
                    students: 62
                },
                {
                    title: 'Academic Listening and Note-taking',
                    price: 26.00,
                    img: require('../../assets/img/stock-full-hd-06-480x298.jpg'),
                    lessons: 14,
                    students: 67
                },
                {
                    title: 'Master jQuery in a Short Period of Time',
                    price: 39.00,
                    img: require('../../assets/img/course-featured-image-01-480x298.jpg'),
                    lessons: 6,
                    students: 51
                },
                {
                    title: 'Introduction to Javascript for Beginners',
                    price: 59.00,
                    img: require('../../assets/img/stock-full-hd-05-480x298.jpg'),
                    lessons: 14,
                    students: 76
                }
            ]
        }
    }
}
</script>

<style lang='scss' scoped>


</style>