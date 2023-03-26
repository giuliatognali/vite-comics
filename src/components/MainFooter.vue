<script>
import MenuFooter from './MenuFooter.vue';
import LogoFooter from './LogoFooter.vue';

export default {
    name: 'MainFooter',
    data() {
        return { }
    },
    components:{
        MenuFooter,
        LogoFooter
    }
}
</script>

<template>
<div class="main-footer">
    <div class="container">
        <MenuFooter/>
        <div class="logo">
        <LogoFooter/>
    </div>
    </div>
    

</div>
</template>

<style lang="scss" scoped>
.main-footer {
    min-height: 370px;
    background-image: url(../assets/img/footer-bg.jpg);
    overflow: hidden;

    .container{
        display: flex;
        justify-content: space-between;
        position: relative;
       

        .logo{
            position: absolute;
           right: 100px;
           top: -100px

        }
    }
}


</style>