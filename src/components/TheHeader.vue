<template>
    <header>
        <nav class="d-flex justify-content-between align-items-center py-3">
            <div>
                <img src="/dc-logo.png" alt="">
            </div>
            <div class="mx-3 ">
                <ul class="d-flex m-0">
                    <li class="p-2"
                    v-for="(listaLinkHTML, i) in listaLinkNav">
                        <a href="">{{listaLinkHTML.testo}}</a>
                    </li>
                </ul>
            </div>
        </nav>
    </header>
</template>

<script>
export default {

    data() {
        return {
            listaLinkNav: [
                {
                    testo: "CHARACTERS",
                },{
                    testo: "COMICS",
                },{
                    testo: "MOVIES",
                },{
                    testo: "TV",
                },{
                    testo: "SGAMES",
                },{
                    testo: "COLLECTIRIES",
                },{
                    testo: "VIDEOS",
                },{
                    testo: "FANS",
                },{
                    testo: "NEWS",
                },{
                    testo: "SHOP",
                },
            ]
        };
    },
    methods: {},
    beforeMount() { },
}
</script>

<style scoped>
    a {
        text-decoration: none;
    }

    img {
        width: 80px;
    }
</style>