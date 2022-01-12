<template>
    <main>
        <DistantLearning/>
        <Courses/>
        <SmartTutoring/>
        <TopLearners/>
    </main>
</template>

<script>
import DistantLearning from '../sections/DistantLearning.vue';
import Courses from '../sections/Courses.vue';
import SmartTutoring from '../sections/SmartTutoring.vue';
import TopLearners from '../sections/TopLearners.vue';

export default {
    name: 'Main',
    components: {
        DistantLearning,
        Courses,
        SmartTutoring,
        TopLearners
    }
}
</script>

<style lang='scss' scoped>

</style>