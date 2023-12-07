<script>
import logo from './logo.vue';
import navbar from './navbar.vue';


export default {
    nome: "header",
    data() {
        return {

        }
    },
    components: {
        logo,
        navbar,
    }
}

</script>

<template>
    <header>
        <div class="contenitore">
            <div>
                <logo></logo>
            </div>
            <div>
                <navbar></navbar>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header {
    padding-bottom: 10px;

    .contenitore {
        width: 80%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-top: 20px;
    }

}
</style>