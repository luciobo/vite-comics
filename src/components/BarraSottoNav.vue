
<template>

    <div>
        <div class="jumbotron-mini">
        </div>
        <div class="container">
            <button class="btn btn-primary button-current-series">CURRENT SERIES</button>
        </div>
        <div class="container ">
            <div class="row g-4 py-4">
                <div class="col-2"
                    v-for="(stampaCard, i) in newEroiDc">
                    <div class="card h-100 bg-card text-light ">
                        <img :src="stampaCard.thumb" class="card-img-top" alt="...">
                        <div class="card-body">
                            <a class="text-light text-decoration-none" href="">{{stampaCard.series}}</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="text-center py-3">
            <button class="btn btn-primary button-load-more">LOAD MORE</button>
        </div>
    </div>

</template>

<script>

import { eroiDcComics } from "../Composables/Array"

export default {

    data() {
        return {
            newEroiDc: eroiDcComics
        };
    },
    methods: {},

    beforeMount() { },

}

</script>

<style scoped>
.jumbotron-mini {
    background-image: url(/jumbotron.jpg);
    height: 400px;
    background-size: cover;
}

.bg-card {
    background-color: #1C1C1C;
    border: none;
}

.button-load-more {
    border-radius: 0;
    padding: .3rem 3rem;
}

.button-current-series {
    border-radius: 0;
    padding: .3rem 1rem;
    position: relative;
    bottom: 18px;
}

</style>