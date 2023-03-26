<script>
import BtnFooter from './BtnFooter.vue';

export default {
    name: 'BottomFooter',
    data() {
        return { }
    },
    components: {
        BtnFooter
    }
}
</script>

<template>
    <div>
        <div>
            <BtnFooter/>
        </div>
        <div>
            icone
        </div>
    </div>

</template>

<style lang="scss" scoped>

@use "../assets/style/partials/variables.scss" as *;
div{
    background-color: $secondary-color;
}
</style>