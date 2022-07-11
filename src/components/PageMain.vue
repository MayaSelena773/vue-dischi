<template>
    <main>
        <div class="albums-container">
            <div class="cards" v-for="album in albumsList" :key="album.index">
                <div class="card">
                    <img class="album-poster" :src="album.poster" :alt="album.author">
                    <h4>{{album.title}}</h4>
                    <h5>{{album.author}}</h5>
                    <h5>{{album.year}}</h5>
                </div>
            </div>
        </div>
    </main>
</template>

<script>
import axios from "axios";

export default {
    name:'PageMain',
    data() {
        return{
            url: "https://flynn.boolean.careers/exercises/api/array/music",
            albumsList: [],
        }
    },
    created(){
        this.getAlbums();
    },
    methods: {
        getAlbums() {
            axios.get(this.url).then((result) => {
                this.albumsList = result.data.response
            });
        }
    }
}

</script>

<style lang="scss" scoped>
@import './style/vars.scss';

main {
    background-color: $brand_secondary_color;
    width: 100%;
    height: auto;
    color: white;

    .albums-container {
        margin: 0 150px;
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
        padding: 2.5rem 0;

        .cards {
            margin: 1rem;

            .card {
            width: 150px;
            height: 270px;
            background-color: $brand_primary_color;
            text-align: center;

                .album-poster {
                    margin: 1rem;
                    width: 120px;
                    height: 120px;
                }

                h4 {
                    text-transform: uppercase;
                    font-weight: bold;
                    margin-bottom: 1rem;
                    padding: 0 10px;
                }

                h5 {
                    color:rgb(121, 125, 125);
                }
            }
        }
    }
}


</style>


