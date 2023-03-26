<script>

export default {
    name: 'TopFooter',
    data() {
        return {}
    }
}
</script>

<template>
    <div class="top-footer">
            <ul class="container">
                <li>
                    <div class="content-list">
                        <a href="#">
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                            <h4>DIGITAL COMICS</h4>
                        </a>
                    </div>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                        <h4>DIGITAL COMICS</h4>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                        <h4>DIGITAL COMICS</h4>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                        <h4>DIGITAL COMICS</h4>
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
            li{ 
                padding: 15px;
                &:hover{
                    border:1px solid white;
                }
            }
            a {
                display: flex;
                align-items: center;

                img {
                    height: 50px;
                    padding-right: 18px;
                }
            }
    }
}
</style>