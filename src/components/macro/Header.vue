<template>
    <header>
        <div class="container">
            <div class="row">

                <!-- logo -->
                <div class="col-3 logo">
                    <img src="../../assets/img/dark-logo.png" alt="MaxCoach logo">
                </div>

                <!-- navbar -->
                <nav class="col-9">
                    <ul>
                        <li v-for="(link, index) in navLinks" :key="index">
                            <a href="#" class="text-color">{{link.title}} <i class="fas fa-chevron-down"></i></a> 
                        </li>
                        <li class="text-color"><i class="far fa-user-circle"></i></li>
                        <li class="custom-search">
                            <input type="text" placeholder="Search...">
                            <button>
                                <i class="fas fa-search"></i>
                            </button>
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

header {
    height: 80px;

    .container, 
    .row {
        height: 100%;
    }

    .logo {
        display: flex;
        align-items: center;

        img {
            height: 40%;
        }
    }

    nav {
        ul {
            height: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;

            a {

                .fa-chevron-down {
                    font-size: .6em;
                    margin-left: 5px;
                }
            }

        }
    }
}

</style>