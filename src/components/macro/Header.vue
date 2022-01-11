<template>
    <header>
        <div class="container">
            <div class="row">

                <!-- logo -->
                <div class="col logo">
                    <img src="../../assets/img/dark-logo.png" alt="MaxCoach logo">
                </div>

                <!-- navbar -->
                <nav class="col">

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
}

</style>