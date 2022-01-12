<template>
    <section class="section-bg-grey">
        <div class="container py-5">
            <div class="row">

                <!-- description -->
                <div class="col-4">

                    <h3 class="sub-title">enjoy insights</h3>
                    <h2 class="mt-2 mb-4 medium-title">Most viewed <span class="text-green">Best Blogs</span></h2>

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

</style>