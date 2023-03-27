<script>

export default {
    name: 'TopFooter',
    data() {
        return {
            buyList: [
                {
                    icon: 'icons/buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS',
                    link: '#'
                },
                {
                    icon: 'icons/buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE',
                    link: '#'
                },
                {
                    icon: 'icons/buy-comics-subscriptions.png',
                    text: 'SUBSCRIPTION',
                    link: '#'
                },
                {
                    icon: 'icons/buy-comics-shop-locator.png',
                    text: 'COMIC SHOP LOCATOR',
                    link: '#'
                },
                {
                    icon: 'icons/buy-dc-power-visa.svg',
                    text: 'CS POWER VISA',
                    link: '#'
                },
            ]
        }
    }
}
</script>

<template>
    <div class="top-footer">
        <ul class="container">
            <li v-for="element in buyList">
                <a :href="element.link">
                    <div class="img-container">
                        <img :src="element.icon" :alt="element.text">
                    </div>

                    <h4>{{ element.text }}</h4>
                </a>
            </li>

        </ul>
    </div>
</template>

<style lang="scss" scoped>
@use "../assets/style/partials/variables.scss" as *;

.top-footer {
    background-color: $primary-color;

    ul {
        display: flex;
        justify-content: space-around;
        align-items: center;
        min-height: 155px;

        li {
            padding: 15px;

            &:hover {
                border: 1px solid white;
            }
        }

        a {
            display: flex;
            align-items: center;

            .img-container {
                height: 50px;
                width: 50px;
                padding-right: 18px;

                img {
                width: 100%;
                height: 100%;
                object-fit: contain;

            }
            }

            
        }
    }
}
</style>