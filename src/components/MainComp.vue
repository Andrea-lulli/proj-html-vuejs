<template>
    <div>
        <section1Comp />
        <section2Comp />
        <section3Comp />
        <section4Comp />
        <section5Comp :latest_post="latest_post" />
        <section6Comp />
    </div>
</template>

<script>

import section1Comp from "./section1Comp.vue";
import section2Comp from "./section2Comp.vue"
import section3Comp from "./section3Comp.vue";
import section4Comp from "./section4Comp.vue";
import section5Comp from "./section5Comp.vue";
import section6Comp from "./section6Comp.vue";


    export default {
        name:'MainComp',
        components: {
    section1Comp,
    section2Comp,
    section3Comp,
    section4Comp,
    section5Comp,
    section6Comp, 
  },
        props: {
    latest_post: Array
  }
    }
</script>

<style lang="scss" scoped>

</style>