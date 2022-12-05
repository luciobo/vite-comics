
<template>

    <div>
        <div class="jumbotron-mini">
        </div>
        <div class="container ">
            <div class="row g-4 py-5">
                <div class="col-2"
                    v-for="(stampaCard, i) in newEroiDc">
                    <div class="card h-100 bg-card text-light ">
                        <img :src="stampaCard.thumb" class="card-img-top" alt="...">
                        <div class="card-body">
                            <h5 class="card-title">{{ stampaCard.series }}</h5>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div>
            
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
</style>