<script>
export default {
    name: "piedipagina",
    data() {
        return {
            icone: ["../../public/img/img/footer-facebook.png", "../../public/img/img/footer-twitter.png",
                "../../public/img/img/footer-youtube.png", "../../public/img/img/footer-pinterest.png",
                "../../public/img/img/footer-periscope.png"]
        }
    }
}
</script>
<template>
    <div class="containerpiedipagina">
        <div class="contenutofooter">
            <div class="registrazione">
                <button>Sign-Up Now!</button>
                <div class="icone">
                    <ul>
                        <h2>Follow us</h2>
                        <li v-for="icona in icone">
                            <img :src="icona" alt="">
                        </li>
                    </ul>
                </div>
            </div>


        </div>
    </div>
</template>
<style lang="scss" scoped>
.containerpiedipagina {
    position: relative;

    .contenutofooter {
        position: absolute;
        width: 100%;
        background-color: #2c2c2c;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 20px 0px;
    }

    .registrazione {
        width: 80%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
    }

    button {
        border: 2px solid #0282f9;
        background-color: #2c2c2c;
        color: white;
        padding: 10px 10px;
        text-transform: uppercase;
        cursor: pointer;
    }

    li {
        display: inline-block;
    }

    img {
        width: 30px;
        margin-left: 15px;
    }
    ul{
        display: flex;
        align-items: center;
    }
    h2{
        color:#0282f9;
        text-transform: uppercase;
        font-size: 16px;
        font-weight: bolder;
        margin-right: 20px;
    }

}</style>