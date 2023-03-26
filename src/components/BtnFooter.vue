<script>
export default {
    name: 'BtnFooter',
    data() {
        return { }
    }
}
</script>

<template>
<div>
    <button>
        <a href="#">SIGN-UP NOW!</a>
    </button>
</div>

</template>

<style lang="scss" scoped>

@use '../assets/style/partials/variables' as *;

button {
    background-color: $secondary-color;
    border: 2px solid $primary-color;
    padding: .9375rem;
    
    &:hover{
        background-color: $primary-color;
    }
    a{
        color:white;
    }
}

</style>