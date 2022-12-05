<template>
    <div class="">
        <div class="row mx-3 d-flex justify-content-between py-5">
            <div class="col-2 d-flex align-items-center"
            v-for="(stampaCardShop, i) in newContenutoCard">
                <img :src="stampaCardShop.icon" alt="">
                <span class="ps-2">
                    <a class="text-light text-decoration-none small" href="">{{stampaCardShop.name}}</a>
                </span>
            </div>
        </div>
    </div>
</template>


<script>

import { itemsBannerMain } from "../Composables/cardShop"

export default {

    data() {
        return {
            newContenutoCard: itemsBannerMain
        };
    },
    methods: {},

    beforeMount() {},

}

</script>

<style scoped>

img {
    width: 50px;
}

</style>