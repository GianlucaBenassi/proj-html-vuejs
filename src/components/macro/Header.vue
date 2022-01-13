<template>
    <header>
        <div class="container">
            <div class="row">

                <!-- logo -->
                <div class="col-8 col-lg-3 logo d-flex align-items-center">
                    <img src="../../assets/img/dark-logo.png" alt="MaxCoach logo">
                </div>

                <!-- navbar large screen-->
                <nav class="col-4 col-lg-9 d-flex justify-content-end align-items-center">
                    <ul class="d-none d-lg-flex justify-content-end">
                        
                        <!-- dynamic links -->
                        <li v-for="(link, index) in navLinks" :key="index" class="ms-2 ms-xl-4">
                            <a href="#" class="text-color d-flex align-items-center">{{link.title}} <i class="fas fa-chevron-down"></i></a>
                            <div class="dropdown">
                                <ul>
                                    <li v-for="text in link.links" :key="text">
                                        <a href="#" class="text-color">{{text}}</a>
                                    </li>
                                </ul>
                            </div>
                        </li>

                        <!-- login icon -->
                        <li class="ms-2 ms-xl-4">
                            <a href="#" class="text-color d-flex align-items-center"><i class="far fa-user-circle"></i></a> 
                        </li>

                        <!-- search bar -->
                        <li class="d-flex align-items-center ms-2 ms-xl-4">
                            <div class="custom-search">
                                <input type="text" placeholder="Search...">
                                <button class="grey">
                                    <i class="fas fa-search"></i>
                                </button>
                            </div>
                        </li>

                    </ul>

                    <!-- menu bars -->
                    <div class="d-lg-none me-3 menu_bars" @click="dataShared.navOpenMenu = !dataShared.navOpenMenu">
                        <i class="fas fa-bars"></i>
                    </div>
                </nav>

            </div>

            <!-- mobile menu -->
            <div v-if="dataShared.navOpenMenu" class="mobile_menu p-4">
                <ul>
                    
                    <!-- login icon -->
                    <li class="mb-3">
                        <a href="#" class="d-flex align-items-center text-color mobile_login">
                            <i class="far fa-user-circle"></i>
                            <span class="ms-2">Login</span>
                        </a>
                    </li>

                    <!-- search bar -->
                    <li class="mb-3 mobile_custom-search">
                        <div class="custom-search">
                            <input type="text" placeholder="Search...">
                            <button class="grey">
                                <i class="fas fa-search"></i>
                            </button>
                        </div>
                    </li>

                    <!-- list title -->
                    <li v-for="(link, index) in navLinks" :key="index">
                        <a href="#" class="d-block mobile_title text-color">{{link.title}}</a>

                        <!-- link list -->
                        <ul class="row row-cols-1 row-cols-sm-2 my-3">
                            <li v-for="(text, index) in link.links" :key="index" class="col mb-2">
                                <a href="#" class="text-color-light hover-text-green">{{text}}</a>
                            </li>
                        </ul>

                    </li>
                </ul>
            </div>

        </div>
    </header>
</template>

<script>
import dataShared from '../../shared/dataShared';

export default {
    name: 'Header',
    props: {
        navLinks: Array
    },
    data() {
        return {
            dataShared
        }
    }
}
</script>

<style lang='scss' scoped>

@import '../../assets/style/_variables.scss';

header {
    height: 80px;
    background-color: #fff;
    box-shadow: 0px 2px 10px 1px rgba(0,0,0,.1);
    position: sticky;
    top: 0;
    z-index: 9999;

    .container, 
    .row {
        height: 100%;
    }

    .logo img {
        height: 40%;
        
    }

    nav {

        // large menu
        & > ul {
            height: 100%;

            & > li {
                // margin-left: 30px;
                position: relative;

                & > a {
                    height: 100%;

                    .fa-chevron-down {
                        font-size: .6em;
                        margin-left: 5px;
                        margin-top: 5px;
                    }
                }

                &:hover > a {
                    color: $mainGreen;
                }

                &:hover .dropdown {
                    display: block;
                }
            }

        }

        .dropdown {
            display: none;
            background-color: #fff;
            position: absolute;
            top: 100%;
            left: -10px;
            padding: 20px 40px 20px 20px;
            border-bottom: 5px solid $mainGreen;
            box-shadow: 0px 0px 10px 0px rgba(0,0,0,0.25);

            & > ul > li {
                white-space: nowrap;
                padding: 10px 0;
                line-height: initial;

                &:hover a {
                    color: $mainGreen;
                }
            }
        }


        // mobile menu bars
        .menu_bars {
            font-size: 20px;
            
            .fa-bars {
                cursor: pointer;
            }
        }

    }

    .mobile_menu {
        background-color: #fff;
        height: calc(100vh - 81px);
        overflow-y: auto;
        position: fixed;
        top: 81px;
        left: 0;
        right: 0;

        .mobile_login {
            font-size: 2rem;

            span {
                font-size: 1.3rem;
                font-weight: bold;
            }
        }

        .mobile_custom-search {
            max-width: 400px;
        }

        .mobile_title {
            font-size: 1.2rem;
            font-weight: bold;
        }
    }
}

</style>