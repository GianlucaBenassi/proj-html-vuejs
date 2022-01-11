<template>
    <main>
        <DistantLearning/>
        <Courses/>
    </main>
</template>

<script>
import DistantLearning from '../sections/DistantLearning.vue';
import Courses from '../sections/Courses.vue';

export default {
    name: 'Main',
    components: {
        DistantLearning,
        Courses
    }
}
</script>

<style lang='scss' scoped>

</style>