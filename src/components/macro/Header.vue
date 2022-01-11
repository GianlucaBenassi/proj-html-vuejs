<template>
    <header>
        <div class="container">
            <div class="row">

                <!-- logo -->
                <div class="col-3 logo d-flex align-items-center">
                    <img src="../../assets/img/dark-logo.png" alt="MaxCoach logo">
                </div>

                <!-- navbar -->
                <nav class="col-9">
                    <ul class="d-flex justify-content-end">
                        
                        <!-- dynamic links -->
                        <li v-for="(link, index) in navLinks" :key="index">
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
                        <li>
                            <a href="#" class="text-color d-flex align-items-center"><i class="far fa-user-circle"></i></a> 
                        </li>

                        <!-- search bar -->
                        <li class="d-flex align-items-center">
                            <div class="custom-search">
                                <input type="text" placeholder="Search...">
                                <button>
                                    <i class="fas fa-search"></i>
                                </button>
                            </div>
                        </li>

                    </ul>
                </nav>

            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header',
    props: {
        navLinks: Array
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
        & > ul {
            height: 100%;

            & > li {
                margin-left: 30px;
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
    }
}

</style>