<script>

export default {
    name: 'CardElement',
    props:{
        img: String,
        name: String,
        link: String
    }

}
</script>

<template>
    <div>
        <a :href="link">
            <img :src="img" :alt="name">
            <p>{{ name }}</p>
        </a>
    </div>
</template>
 

<style lang="scss" scoped></style>