<script>
export default {
    name: 'ComicList'
}
</script>

<template>
    <section>
        <div class="container">
            <div class="label">
                <h2>CURRENT SERIES</h2>
            </div>
            <div class="container-small">
                <div class="card-comic">
                    CARD
                </div>
                <div class="card-comic">
                    CARD
                </div>
                <div class="card-comic">
                    CARD
                </div>
                <div class="card-comic">
                    CARD
                </div>
                <div class="card-comic">
                    CARD
                </div>
                <div class="card-comic">
                    CARD
                </div>
                <div class="card-comic">
                    CARD
                </div>
                <div class="card-comic">
                    CARD
                </div>
            </div>
            <div class="container">
                <button class="btn-load">
                    <h4>LOAD MORE</h4>
                </button>

            </div>
        </div>

    </section>
</template>


<style lang="scss" scoped>
@use "../assets/style/partials/variables.scss" as *;

section {
    background-color: #1c1c1c;

    .container {
        position: relative;

        .label {
            background-color: $primary-color;
            border: none;
            color: white;
            padding: 15px 30px;
            position: absolute;
            top: -20px;
        }

        .container-small {
            background-color: pink;
            display: flex;
            align-items: center;
            flex-wrap: wrap;
            padding-top: 60px;


            .card-comic {
                background-color: $primary-color;
                width: calc(100% / 6);
                height: 220px;
                margin: 10px 15px;

            }

        }
.container{
    display: flex;
    justify-content: center;
    
    .btn-load {
                background-color: $primary-color;
                height: 40px;
                width: 185px;
                border: none;
                color: white;
                padding: 15px 30px;
            
                margin: 20px;
            }
}

    }
}
</style>