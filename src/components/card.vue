<script>
export default{
    props:["immagine", "nome"],
    name:"card",
    data(){
        return
    },
}
</script>
<template>
    <li>
        <figure>
            <img :src="immagine" :alt="nome">
        </figure>
        <div class="nomeserie">
            {{ nome }}
        </div>   
    </li>
</template>
<style lang="scss" scoped>
li {
    flex-basis: calc((100% / 6) - 20px);
    margin-bottom: 30px;
    margin-left: 20px;
}

figure {
    height: 300px;
}
img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center top;
}

.nomeserie{
        margin-top: 20px;
        color: white;
    }
</style>