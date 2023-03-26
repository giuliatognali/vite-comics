<script>
import BottomFooter from './BottomFooter.vue';
import MainFooter from './MainFooter.vue';

export default{
    name: 'AppFooter',
    data() {
        return {}
    },
    components: {
        BottomFooter,
        MainFooter
    }
}
</script>

<template>
   <footer>
    <MainFooter/>
    <BottomFooter />
    
</footer>
</template>

<style lang="scss" scoped></style>