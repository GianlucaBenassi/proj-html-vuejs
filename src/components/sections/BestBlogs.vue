<template>
    <section class="section-bg-grey">
        <div class="container py-5">
            <div class="row">

                <!-- description -->
                <div class="col-4">

                    <h3 class="sub-title">enjoy insights</h3>
                    <h2 class="mt-3 mb-5 medium-title">Most viewed <span class="text-green">Best Blogs</span></h2>

                    <ul>
                        <li class="hover-text-green mb-4"><a href="#" class="text-color hover-text-green">Become a Better Blogger: Content Planning</a></li>
                        <li class="hover-text-green mb-4"><a href="#" class="text-color hover-text-green">Promoting Your Online Business on Pinterest</a></li>
                        <li class="hover-text-green mb-4"><a href="#" class="text-color hover-text-green">Gamification and Game-Based Learning</a></li>
                        <li class="hover-text-green mb-4"><a href="#" class="text-color hover-text-green">Designing an Online Course from Expert's Persective</a></li>
                        <li class="hover-text-green mb-4"><a href="#" class="text-color hover-text-green">Why Online Courses Are the Future of Education</a></li>
                    </ul>

                </div>

                <!-- posts -->
                <div class="col-8">

                    <div class="row">

                        <div class="col px-5">
                            <div class="blog_post">

                                <div class="image">
                                    <img src="../../assets/img/artist-blog-03-480x352.jpeg" alt="artist blog 01" class="d-block">
                                </div>

                                <div class="desc p-4">
                                    <span class="type text-color-light hover-text-green">artist</span>
                                    <h5 class="text-gunPowder hover-text-green mt-3 mb-4">Brush Strokes Energize Trees in Paintings</h5>
                                    <span class="date d-inline-block text-color-light me-5"><i class="far fa-calendar"></i> May 15, 2020</span>
                                    <span class="views d-inline-block text-color-light"><i class="fas fa-eye"></i> 668 views</span>
                                </div>

                            </div>
                        </div>

                        <div class="col px-5">
                            <div class="blog_post">

                                <div class="image">
                                    <img src="../../assets/img/artist-blog-01-480x352.jpg" alt="artist blog 02" class="d-block">
                                </div>

                                <div class="desc p-4">
                                    <span class="type text-color-light hover-text-green">artist</span>
                                    <h5 class="text-gunPowder hover-text-green mt-3 mb-4">Poket-Sized Notebooks Hold Miniature Paintings</h5>
                                    <span class="date d-inline-block text-color-light me-5"><i class="far fa-calendar"></i>May 15, 2020</span>
                                    <span class="views d-inline-block text-color-light"><i class="fas fa-eye"></i>603 views</span>
                                </div>

                            </div>
                        </div>

                    </div>

                </div>

            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'BestBlogs'
}
</script>

<style lang='scss' scoped>

h2 span {
    font-weight: normal;
}

li a {
    font-weight: bold;
}

li::before {
    font-family: "Font Awesome 5 Free"; 
    font-weight: 900;
    content: "\f30b";
    padding-right: 10px;
}


.blog_post {
    border-radius: 5px;
    overflow: hidden;

    .image {
        overflow: hidden;

        img {
            width: 100%;
            cursor: pointer;
            transition: .8s;
        }

        &:hover img {
            transform: scale(1.1);
        }
    }

    .desc {
        background-color: #fff;

        .type {
            text-transform: uppercase;
            cursor: pointer;
        }

        h5 {
            font-size: 1.4rem;
            cursor: pointer;
        }

        .date,
        .views {
            font-size: .8rem;
        }

        .fa-calendar,
        .fa-eye {
            margin-right: 6px;
        }
    }
}

</style>