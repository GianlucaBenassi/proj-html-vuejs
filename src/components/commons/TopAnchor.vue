<template>
    <div @click="scroolToTop()" class="d-flex justify-content-center align-items-center top_anchor bg-green">
        <i class="fas fa-long-arrow-alt-up"></i>
    </div>
</template>

<script>
export default {
    name: 'TopAnchor',
    methods: {
        scroolToTop() {
            window.scrollTo({top: 0, behavior: 'smooth'});
        }
    }
}
</script>

<style lang='scss' scoped>

.top_anchor {
    width: 50px;
    height: 50px;
    color: #fff;
    font-size: 20px;
    border-radius: 50%;
    position: absolute;
    bottom: 10px;
    right: 10px;
    z-index: 9998;
    cursor: pointer;
}

</style>