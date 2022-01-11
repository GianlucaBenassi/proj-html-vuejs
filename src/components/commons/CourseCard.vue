<template>
    <div class="row">

        <!-- image -->
        <div class="col-auto">
            <img src="../../assets/img/course-02-480x298.jpg" alt="course_01">
        </div>

        <!-- infos -->
        <div class="col d-flex flex-column justify-content-center">
            <span class="price text-green">$40<span class="cents">.00</span></span>
            <h4 class="my-3">Learning to Write as a Professional Author</h4>
            <div class="infos">
                <span class="text-color-light me-5"><i class="far fa-file-alt"></i> 20 Lessons</span>
                <span class="text-color-light"><i class="far fa-user"></i> 50 Students</span>
            </div>
        </div>

    </div>
</template>

<script>
export default {
    name: 'CorseCard'
}
</script>

<style lang='scss' scoped>

img {
    width: 170px;
    height: 170px;
    border-radius: 50%;
    object-fit: cover;
}

.price {
    font-weight: bold;
    font-size: 1.3rem;

    .cents {
        font-size: initial;
    }
}

.fa-file-alt,
.fa-user {
    margin-right: 6px;
}

</style>