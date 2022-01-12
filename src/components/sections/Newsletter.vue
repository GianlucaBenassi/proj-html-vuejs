<template>
    <section>
        <div class="container text-center py-5">

            <h2 class="mt-2 mb-4 medium-title">Subscribe <span class="text-green">Newsletters</span></h2>
            <p class="text-color-light">Enter your email address to register to our newsletter subscribtion delivered on a regular basis!</p>

            <!-- custom searchbar -->
            <div class="d-flex justify-content-center my-5">
                <div class="custom-search">
                    <input type="text" placeholder="Enter your email">
                    <button class="green">
                        Subscribe
                    </button>
                </div>
            </div>

            <!-- shapes -->
            <img src="../../assets/img/maxcoach-shape-02.png" alt="shape 01" class="shape sh-01">
            <img src="../../assets/img/maxcoach-shape-09.png" alt="shape 02" class="shape sh-02">
            <div class="circle-shape green shape"></div>

        </div>
    </section>
</template>

<script>
export default {
    name: 'Newsletter'
}
</script>

<style lang='scss' scoped>

.container {
    position: relative;
}

.custom-search {
    width: 30%;
}

.shape {
    position: absolute;

    &.sh-01 {
        top: 40%;
        right: 10%;
    }
    
    &.sh-02 {
        top: 5%;
        right: 10%;
    }

    &.circle-shape {
        top: 45%;
        left: 10%;
    }
}

</style>