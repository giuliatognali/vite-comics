<script>

export default {
    name: 'MenuFooter',
    data() {
        return {
            menu: [
                {
                    menuName: 'DC COMICS',
                    content: [
                        {
                            text: 'Characters',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Comics',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Movies',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'TV',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Games',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Videos',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'News',
                            link: '#',
                            target: '_blank'
                        }
                    ]
                },
                {
                    menuName: 'SHOP',
                    content: [
                        {
                            text: 'Shop DC',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Shop DC collectibles',
                            link: '#',
                            target: '_blank'
                        }
                    ]
                },
                {
                    menuName: 'DC',
                    content: [
                        {
                            text: 'Terms Of Use',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Privacy policy (New)',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Ad Choices',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Advertising',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Jobs',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Subscriptions',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Talent Workshops',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'CPSC Certificates',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Ratings',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Shop Help',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Contact Us',
                            link: '#',
                            target: '_blank'
                        }
                    ]
                },
                {
                    menuName: 'SITES',
                    content: [
                        {
                            text: 'DC',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'MAD Magazine',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'DC Kids',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'DC Universe',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'DC Power Visa',
                            link: '#',
                            target: '_blank'
                        }
                    ]
                }
            ]
        }
    }
}
</script>

<template>
    <div>
    <ul v-for="element in menu">
        <h3>{{ element.menuName }}</h3>
        <li v-for="listItem in element.content">
            <a :href="listItem.link" :target="listItem.target">{{ listItem.text }}</a>
        </li>
    </ul>
</div>
</template>

<style lang="scss" scoped>

@use "../assets/style/partials/variables.scss" as *;

div{
    display: flex;
    flex-direction: column;
    max-height: 23.125rem;
    flex-wrap: wrap;
    padding-top: 25px;
    max-width: 40%;
    
    ul{
        padding-top:15px;
        padding-right: 20px;
    }
}
h3 {
    color: white;
    font-stretch: condensed;
    padding-bottom: 25px
}

a{
    font-size: 12px;
    color: $secondary-text-color;
  
}
</style>