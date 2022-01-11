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
                            <a href="#">{{link.title}}</a>
                        </li>
                        <li>LoginImage</li>
                        <li>TextBar</li>
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
        }
    }
}

</style>