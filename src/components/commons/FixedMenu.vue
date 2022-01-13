<template>
    <div class="fix_menu">
        <ul>
            
            <li>
                <a href="#" class="d-flex justify-content-center align-items-center text-color">
                    <i class="fas fa-ruler-combined"></i>
                </a>
            </li>

            <li>
                <a href="#" class="d-flex justify-content-center align-items-center text-color">
                    <i class="far fa-dot-circle"></i>
                </a>
            </li>

            <li>
                <a href="#" class="d-flex justify-content-center align-items-center text-color">
                    <i class="fas fa-book"></i>
                </a>
            </li>

            <li>
                <a href="#" class="d-flex justify-content-center align-items-center text-color">
                    <i class="fas fa-shopping-cart"></i>
                </a>
            </li>

        </ul>
    </div>
</template>

<script>
export default {
    name: 'FixedMenu'
}
</script>

<style lang='scss' scoped>

.fix_menu {
    background-color: #fff;
    box-shadow: -2px 0px 10px 1px rgba(0,0,0,0.1);
    border-top-left-radius: 5px;
    border-bottom-left-radius: 5px;
    position: fixed;
    top: 250px;
    right: 0;
    z-index: 9990;

    li {
       width: 40px;
       height: 40px;

       a {
           width: 100%;
           height: 100%;
       }
    }
    
}

</style>