<template>
    <main>
        <DistantLearning/>
        <Courses/>
        <SmartTutoring/>
    </main>
</template>

<script>
import DistantLearning from '../sections/DistantLearning.vue';
import Courses from '../sections/Courses.vue';
import SmartTutoring from '../sections/SmartTutoring.vue';

export default {
    name: 'Main',
    components: {
        DistantLearning,
        Courses,
        SmartTutoring
    }
}
</script>

<style lang='scss' scoped>

</style>