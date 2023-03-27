<script>
import CardElement from "./CardElement.vue";
export default {
    name: 'ComicList',
    components: {
        CardElement
    },
    data() {
        return {
            comics: [
                {
                    "thumb": "https://static.dc.com/2023-03/LEGIONOB_Cv1_00111_DIGITAL.jpg?w=640",
                    "link": "#",
                    "series": "DC'S LEGION OF BLOOM",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/FLS_Cv795_79511_DIGITAL.jpg?w=640",
                    "link": "#",
                    "series": "THE FLASH",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/NTW_Cv102_10211_DIGITAL-1.jpg?w=640",
                    "link": "#",
                    "series": "NIGHTWING",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/BMSMWF_Cv13_01311_DIGITAL.jpg?w=640",
                    "link": "#",
                    "series": "BATMAN/SUPERMAN: WORLD'S FINEST",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/CTW_Cv53_05311_DIGITAL.jpg?w=640",
                    "link": "#",
                    "series": "CATWOMAN",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/BA_Cv9_00911_DIGITAL.jpg?w=640",
                    "link": "#",
                    "series": "BLACK ADAM",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/SM_LOST_Cv1_00111_DIGITAL.jpg?w=640",
                    "link": "#",
                    "series": "SUPERMAN: LOST",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/SUPES_Cv2_00211_DIGITAL.jpg?w=640",
                    "link": "#",
                    "series": "SUPERMAN",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/ROBIN_v3%20%28Cover%29.jpg?w=640",
                    "link": "#",
                    "series": "ROBIN VOL. 3: SECRETS AND SHADOWS ",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/HQv3%20%28%20Cover%29.jpg?w=640",
                    "link": "#",
                    "series": "HARLEY QUINN VOL. 3: VERDICT",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/MULTVTJ%20%28COVER%29.jpg?w=640",
                    "link": "#",
                    "series": "MULTIVERSITY: TEEN JUSTICE",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/WW_Cv797_79711_DIGITAL.jpg?w=640",
                    "link": "#",
                    "series": "WONDER WOMAN",
                    "type": "graphic novel"
                }
            ]
        }
    }
}
</script>

<template>
    <section>
        <div class="container">
            <div class="label">
                <h2>CURRENT SERIES</h2>
            </div>
            <div class="container-small">
                <CardElement 
                class="card-comic" 
                v-for="comic in comics" 
                :link="comic.link"
                :img="comic.thumb"
                :name="comic.series"
                />
                
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
            display: flex;
            align-items: flex-start;
            flex-wrap: wrap;
            padding-top: 60px;

        }

        .container {
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

.card-comic {
    width: calc((100% / 6) - 30px);
    color: white;
    margin: 10px 15px;
}


</style>