<template>
    <main>
        <DistantLearning/>
        <Courses/>
        <SmartTutoring/>
        <TopLearners/>
        <Data/>
    </main>
</template>

<script>
import DistantLearning from '../sections/DistantLearning.vue';
import Courses from '../sections/Courses.vue';
import SmartTutoring from '../sections/SmartTutoring.vue';
import TopLearners from '../sections/TopLearners.vue';
import Data from '../sections/Data.vue';

export default {
    name: 'Main',
    components: {
        DistantLearning,
        Courses,
        SmartTutoring,
        TopLearners,
        Data
    }
}
</script>

<style lang='scss' scoped>

</style>