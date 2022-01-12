<template>
    <footer class="section-bg-grey">
        <div class="container py-5">
            <div class="row mb-5">

                <!-- address + socials column -->
                <div class="col-6">
                    <h4 class="text-color mb-3">Adress</h4>
                    <span class="d-block text-color-light mb-3">382 NE 191st St # 87394 Miami, FL 33179-3899</span>
                    <span class="d-block text-color-light mb-3">+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)</span>
                    <a href="#" class="d-block text-color-light hover-text-green mb-3">support@maxcoach.com</a>
                    <ul class="d-flex socials">
                        <li class="me-5"><a href="#" class="text-color-light hover-text-green"><i class="fab fa-facebook-square"></i></a></li>
                        <li class="me-5"><a href="#" class="text-color-light hover-text-green"><i class="fab fa-twitter"></i></a></li>
                        <li class="me-5"><a href="#" class="text-color-light hover-text-green"><i class="fab fa-instagram"></i></a></li>
                        <li class="me-5"><a href="#" class="text-color-light hover-text-green"><i class="fab fa-linkedin"></i></a></li>
                    </ul>
                </div>

                <!-- dynamic links column -->
                <div class="col" v-for="(link, index) in footerLinks" :key="index">
                    <h4 class="text-color mb-3">{{link.title}}</h4>
                    <ul :class="'dynamic_list--' + index ">
                        <li class="mb-3" v-for="(text, i) in link.links" :key="i">
                            <a href="#" class="text-color-light hover-text-green">{{text}}</a>
                        </li>
                    </ul>
                </div>

            </div>

            <!-- copyright -->
            <p class="text-color-light text-center"><i class="far fa-copyright"></i> 2020 Maxcoach. All Rights Reserved</p>

        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    props: {
        footerLinks: Array
    }
}
</script>

<style lang='scss' scoped>

footer {
    font-size: .9rem;
}

h4 {
    font-size: 1.1rem;
}

.socials {
    font-size: 1.6rem;
}

.dynamic_list--0{
    display: flex;
    flex-wrap: wrap;
    
    li {
        width: 50%;
    }
}

</style>