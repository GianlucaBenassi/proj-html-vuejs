<template>
    <section class="section-bg-grey">
        <div class="container py-5">
            <div class="row">

                <!-- description -->
                <div class="col-12 col-lg-4 mb-5 mb-lg-8" :class="{'text-center' : dataShared.mdScreen}">

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
                <div class="col-12 col-lg-8">

                    <div class="row row-cols-1 row-cols-md-2">

                        <div class="col px-1 px-md-3 px-xl-5 mb-5 mb-md-0">
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

                        <div class="col px-1 px-md-3 px-xl-5">
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
import dataShared from '../../shared/dataShared';

export default {
    name: 'BestBlogs',
    data() {
        return {
            dataShared
        }
    }
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
    height: 100%;
    background-color: #fff;
    border-radius: 5px;

    .image {
        overflow: hidden;
        border-top-left-radius: 5px;
        border-top-right-radius: 5px;

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
        border-bottom-left-radius: 5px;
        border-bottom-right-radius: 5px;

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