<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            menu{
                characherts,
            }

        }
    }
}
</script>

<!-- html -->
<template>
    <nav>
        <div>
            Logo
        </div>
        <div>
            <ul>
                <li>MENU</li>
                <li>MENU</li>
                <li>MENU</li>
                <li>MENU</li>
                <li>MENU</li>
                <li>MENU</li>
                <li>MENU</li>
                <li>MENU</li>
                <li>MENU</li>
                <li>MENU</li>
            </ul>
        </div>
    </nav>
</template>

<style lang="scss" scoped>

@use "../style/variables.scss" as *;
nav{
    height: 4.6875rem;
    max-width: 80rem;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center ;
    

    ul{
        display: flex;
        justify-content: center;
        list-style: none;

        li{
            color: $secondary-color;
            display: inline-block;
            
            &:hover{
                border-bottom: 2px solid $primary-color;
            }
        }

    }
}

</style>