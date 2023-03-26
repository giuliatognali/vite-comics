<script>
import BtnFooter from './BtnFooter.vue';
import SocialContacts from './SocialContacts.vue';

export default {
    name: 'BottomFooter',
    data() {
        return { }
    },
    components: {
        BtnFooter,
        SocialContacts
        
    }
}
</script>

<template>
    <div class="bottom-footer">
        <div class="container">
            <BtnFooter/>
            <SocialContacts/>
        </div>

           
    </div>

</template>

<style lang="scss" scoped>

@use "../assets/style/partials/variables.scss" as *;
div{
    background-color: $secondary-color;
}

.container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    min-height: 110px;
}
</style>