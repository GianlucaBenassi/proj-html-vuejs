<template>
    <div class="row py-3 ms_card">

        <!-- image -->
        <div class="col-auto">
            <img :src="courseInfo.img" :alt="courseInfo.title">
        </div>

        <!-- infos -->
        <div class="col d-flex flex-column justify-content-center">

            <!-- check price -->
            <span v-if="getPrice != null" class="price text-green">
                ${{getPrice}}<span class="cents">.{{getCents}}</span>
            </span>
            <span v-else class="price text-green">{{courseInfo.price}}</span>
            
            <h4 class="mt-3 mb-2 hover-text-green">{{courseInfo.title}}</h4>
            <div class="d-flex flex-wrap">
                <span class="text-color-light mt-2 me-5"><i class="far fa-file-alt"></i> {{courseInfo.lessons}} Lessons</span>
                <span class="text-color-light mt-2"><i class="far fa-user"></i> {{courseInfo.students}} Students</span>
            </div>
        </div>

    </div>
</template>

<script>
export default {
    name: 'CorseCard',
    props: {
        courseInfo: Object
    },
    computed: {
        getPrice() {
            if (typeof(this.courseInfo.price) == 'number') {
                return this.courseInfo.price.toString().split('.')[0];
            }

            return null;
        },
        getCents() {
            if (typeof(this.courseInfo.price) == 'number') {
                if (this.courseInfo.price.toString().split('.')[1] == null) {
                    return '00';
                } else {
                    return this.courseInfo.price.toString().split('.')[1];
                }
            }

            return null;
        }
    }
}
</script>

<style lang='scss' scoped>

.ms_card {
    border-radius: 5px;
    cursor: pointer;
    transition: all .3s;

    &:hover {
        background-color: #fff;
    }
}

img {
    width: 170px;
    height: 170px;
    border-radius: 50%;
    object-fit: cover;
}

.price {
    font-weight: bold;
    font-size: 1.5rem;

    .cents {
        font-size: initial;
    }
}

h4 {
    font-size: 1.2rem;
    transition: all .3s;
}

.fa-file-alt,
.fa-user {
    margin-right: 6px;
}

</style>