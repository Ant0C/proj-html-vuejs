<script>
import Section1 from './Section1.vue';
import Section2 from './Section2.vue';
import Section3 from './Section3.vue';
import Section4 from './Section4.vue';
import Section5 from './Section5.vue';
import Section6 from './Section6.vue';

export default {
    components: {
        Section1,
        Section2,
        Section3,
        Section4,
        Section5,
        Section6
    },
}

</script>

<template>
    <Section1></Section1>
    <Section2></Section2>
    <Section3></Section3>
    <Section4></Section4>
    <Section5></Section5>
    <Section6></Section6>
</template>

<style lang="scss" scoped>
@use '../src/style/general.scss' as *;
</style>
