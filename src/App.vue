<script>
import main1 from './components/main1.vue';
import header1 from './components/header1.vue';
import footer1 from './components/footer1.vue';


export default {
  data() {
    return {

    }
  },
  components: {
    header1,
    main1,
    footer1,
  },
}

</script>

<template>
  <header1 />
  <main1 />
  <footer1 />
</template>

<style lang="scss" scoped>
@use 'style.scss' as *;

</style>
