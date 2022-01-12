<template>
    <main>
        <DistantLearning/>
        <Courses/>
        <SmartTutoring/>
        <TopLearners/>
        <Data/>
        <BestBlogs/>
        <Newsletter/>
    </main>
</template>

<script>
import DistantLearning from '../sections/DistantLearning.vue';
import Courses from '../sections/Courses.vue';
import SmartTutoring from '../sections/SmartTutoring.vue';
import TopLearners from '../sections/TopLearners.vue';
import Data from '../sections/Data.vue';
import BestBlogs from '../sections/BestBlogs.vue';
import Newsletter from '../sections/Newsletter.vue';

export default {
    name: 'Main',
    components: {
        DistantLearning,
        Courses,
        SmartTutoring,
        TopLearners,
        Data,
        BestBlogs,
        Newsletter
    }
}
</script>

<style lang='scss' scoped>

</style>