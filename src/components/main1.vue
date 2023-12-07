<script>
import content from './content.vue';
import info from './info.vue';


export default {
    nome: "main",
    components: {
        content,
        info
    }

}
</script>

<template>
    <main>
        <content></content>
        <info></info>
    </main>
</template>

<style lang="scss" scoped></style>