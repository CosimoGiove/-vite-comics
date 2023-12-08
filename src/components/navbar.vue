<script>
export default {
    name: "navabr",
    data() {
        return {
            lista: [
                {
                    selezione: "Characters"
                },
                {
                    selezione: "Comics"
                },
                {
                    selezione: "Movies"
                },
                {
                    selezione: "Tv"
                },
                {
                    selezione: "Games"
                },
                {
                    selezione: "Collectibles"
                },
                {
                    selezione: "Videos"
                },
                {
                    selezione: "Fans"
                },
                {
                    selezione: "News"
                },
                {
                    selezione: "Shop"
                },
            ]
        }
    }
}

</script>
<template>
    <ul>
        <li v-for="list in lista">
           <div>{{ list.selezione }}</div>
        </li>
    </ul>
</template>
<style lang="scss" scoped>
ul {
    li {
        display: inline-block;
        margin-left: 30px;
        cursor: pointer;
        text-transform: uppercase;
        font-size: 13px;
        line-height: 77px;
        
    }
    li:hover {
        color: #238efa;
        border-bottom: 3px solid #238efa;
    }
}
</style>