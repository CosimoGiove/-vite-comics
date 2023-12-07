<script>
export default {
    name: "info1",
    data() {
        return {
            informazioni: [
                {
                    img: "../../public/img/img/buy-comics-digital-comics.png",
                    testo: "digital comics"
                },
                {
                    img: "../../public/img/img/buy-comics-merchandise.png",
                    testo: "Dc merchandise"
                },
                {
                    img: "../../public/img/img/buy-comics-subscriptions.png",
                    testo: "subscription"
                },
                {
                    img: "../../public/img/img/buy-comics-shop-locator.png",
                    testo: "comic shop locator"
                },
                {
                    img: "../../public/img/img/buy-dc-power-visa.svg",
                    testo: "dc power visa"
                },
            ]
        }
    }
}

</script>
<template>
    <div class="contenitore">
        <ul>
            <li v-for="(info, index) in informazioni ">
                <div>
                    <img :src="info.img" alt="immagine">
                </div>
                <div>
                    {{ info.testo }}
                </div>

            </li>
        </ul>
    </div>
</template>
<style lang="scss" scoped>
.contenitore {
    background-color: #0282f9;
    padding-top: 40px;
    padding-bottom: 40px;

    ul {
        width: 80%;
        margin: 0 auto;
        display: flex;
        align-items: center;
        justify-content: space-between;

        li {
            display: inline-block;
            display: flex;
            align-items: center;
            color: white;
        }

        img {
            width: 40px;
            margin-right: 15px;
        }
    }
}
</style>