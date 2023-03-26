<script>
import BottomFooter from './BottomFooter.vue';
import MainFooter from './MainFooter.vue';
import TopFooter from './TopFooter.vue';

export default{
    name: 'AppFooter',
    data() {
        return {}
    },
    components: {
        BottomFooter,
        MainFooter,
        TopFooter
    }
}
</script>

<template>
   <footer>
    <TopFooter/>
    <MainFooter/>
    <BottomFooter />
    
</footer>
</template>

<style lang="scss" scoped></style>