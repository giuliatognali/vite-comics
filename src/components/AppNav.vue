<script>

export default {
    name: 'AppNav',
    data() {
        return {
            menuList: [
                {
                    name: 'CHARACTERS',
                    link: '#',
                    target: '_self'
                },
                {
                    name: 'COMICS',
                    link: '#',
                    target: '_self'
                },
                {
                    name: 'MOVIES',
                    link: '#',
                    target: '_self'
                },
                {
                    name: 'TV',
                    link: '#',
                    target: '_self'
                },
                {
                    name: 'GAMERS',
                    link: '#',
                    target: '_self'
                },
                {
                    name: 'COLLECTIBLES',
                    link: '#',
                    target: '_self'
                },
                {
                    name: 'VIDEOS',
                    link: '#',
                    target: '_self'
                },
                {
                    name: 'FANS',
                    link: '#',
                    target: '_self'
                },
                {
                    name: 'NEWS',
                    link: '#',
                    target: '_self'
                },
                {
                    name: 'SHOP',
                    link: '#',
                    target: '_self'
                }
            ]

        }
    }
}
</script>

<!-- html -->
<template>
    <nav>
        <ul>
            <li v-for="element in menuList">
                <a :href="element.link" :target="element.target">{{ element.name }}</a>
            </li>

        </ul>
    </nav>
</template>


<style lang="scss" scoped>
@use "../assets/style/partials/variables.scss" as *;

    ul {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100px;

        li {
            display: flex;
            align-items: center;
            padding: .9375rem;
            height: 100%;

            a {
                font-weight: 600;
                font-stretch: condensed;
                color: $secondary-color;
            }

            &:hover {
                border-bottom: 4px solid $primary-color;

                a {
                    color: $primary-color;
                }

            }
        }

    }
</style>