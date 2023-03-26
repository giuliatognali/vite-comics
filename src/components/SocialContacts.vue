<script>
export default {
    name: 'SocialContacts',
    data() {
        return {
            SocialLinks: [
                {
                    name: 'Facebook',
                    link: '#',
                    icon: 'icons/footer-facebook.png',
                    target: '_blank'

                },
                {
                    name: 'Twitter',
                    link: '#',
                    icon: 'icons/footer-twitter.png',
                    target: '_blank'

                },
                {
                    name: 'You-tube',
                    link: '#',
                    icon: 'icons/footer-youtube.png',
                    target: '_blank'

                },
                {
                    name: 'Pinterest',
                    link: '#',
                    icon: 'icons/footer-pinterest.png',
                    target: '_blank'

                },
                {
                    name: 'Periscope',
                    link: '#',
                    icon: 'icons/footer-periscope.png',
                    target: '_blank'

                }
            ]
        }
    }
}
</script>

<template>
    <div>
        <ul>
            <h3>FOLLOW US</h3>
            <li v-for="link in SocialLinks">
                <a :href="link.link" :target="link.target">
                    <img :src="link.icon" :alt="link.name">
                </a>
            </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;

ul {
    display: flex;
    justify-content: center;
    align-items: center;

            img{
            height:2.1875rem;
            margin: .3125rem;
        }

    h3 {
        color: $primary-color;
        padding: 0 1.5625rem;
    }
}
</style>