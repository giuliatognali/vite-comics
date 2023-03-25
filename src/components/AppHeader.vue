<script>

import AppLogo from './AppLogo.vue';

export default{
    name: 'AppHeader',
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
    },
    components: {
        AppLogo
    }
    }
</script>

<!-- html -->
<template>
    <nav>
        <div>
            <AppLogo/>
        </div>
        <div>
            <ul>
                <li v-for="element in menuList">
                    <a :href="element.link" :target="element.target">{{ element.name }}</a>
                </li>

            </ul>
        </div>
    </nav>
</template>


<style lang="scss" scoped>
@use "../assets/style/partials/variables.scss" as *;

nav {
    height: 6.25rem;
    max-width: 80rem;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;

    ul {
        display: flex;
        justify-content: center;
        list-style: none;

        li {

            display: inline-block;
            padding: .9375rem;

            a {
                color: $secondary-color;
                text-decoration: none;
            }

            &:hover {
                border-bottom: 3px solid $primary-color;

                a {
                    color: $primary-color;
                }

            }
        }

    }
}
</style>