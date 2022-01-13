<template>
    <div class="fix_menu">
        <ul>
            
            <li>
                <a href="#" class="d-flex justify-content-center align-items-center text-color">
                    <i class="fas fa-ruler-combined"></i>
                    <div class="baloon px-3 py-2">
                        <span>Select Demo</span>
                        <div class="corner"></div>
                    </div>
                </a>
            </li>

            <li>
                <a href="#" class="d-flex justify-content-center align-items-center text-color">
                    <i class="far fa-dot-circle"></i>
                    <div class="baloon px-3 py-2">
                        <span>Support Channel</span>
                        <div class="corner"></div>
                    </div>
                </a>
            </li>

            <li>
                <a href="#" class="d-flex justify-content-center align-items-center text-color">
                    <i class="fas fa-book"></i>
                    <div class="baloon px-3 py-2">
                        <span>Documentation</span>
                        <div class="corner"></div>
                    </div>
                </a>
            </li>

            <li>
                <a href="#" class="d-flex justify-content-center align-items-center text-color">
                    <i class="fas fa-shopping-cart"></i>
                    <div class="baloon px-3 py-2">
                        <span>Purchase Maxcoach</span>
                        <div class="corner"></div>
                    </div>
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
            position: relative;

            .baloon {
                display: none;
                background-color: #000;
                box-shadow: 0px 0px 10px 5px rgba(0,0,0,.2);
                border-radius: 5px;
                position: absolute;
                top: 50%;
                right: 140%;
                transform: translate(0, -50%);

                span {
                    color: #fff;
                    font-size: .9rem;
                    font-weight: bold;
                    white-space: nowrap;
                }

                .corner {
                    width: 15px;
                    height: 15px;
                    background-color: black;
                    box-shadow: 0px 0px 10px 5px rgba(0,0,0,.2);
                    position: absolute;
                    top: 50%;
                    right: -5px;
                    transform: translate(0, -50%) rotate(45deg);
                }
            }

            &:hover .baloon {
                display: block;
            }
        }
    }
    
}

</style>