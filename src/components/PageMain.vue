<template>
    <main>
        <div class="albums-container">
            <div class="cards">
                <div class="card">
                    <img src="" alt="">
                    <h4>Ciao</h4>
                </div>

                <div class="card">
                    <img src="" alt="">
                    <h4>Ciao</h4>
                </div>

                <div class="card">
                    <img src="" alt="">
                    <h4>Ciao</h4>
                </div>

                <div class="card">
                    <img src="" alt="">
                    <h4>Ciao</h4>
                </div>

                <div class="card">
                    <img src="" alt="">
                    <h4>Ciao</h4>
                </div>

                <div class="card">
                    <img src="" alt="">
                    <h4>Ciao</h4>
                </div>

                <div class="card">
                    <img src="" alt="">
                    <h4>Ciao</h4>
                </div>

                <div class="card">
                    <img src="" alt="">
                    <h4>Ciao</h4>
                </div>

                <div class="card">
                    <img src="" alt="">
                    <h4>Ciao</h4>
                </div>

                <div class="card">
                    <img src="" alt="">
                    <h4>Ciao</h4>
                </div>
            </div>
        </div>
    </main>
</template>

<script>
export default {
    name:'PageMain'
}
</script>

<style lang="scss" scoped>
main {
    background-color: lightgrey;
    width: 100%;
    height: auto;

    .albums-container {
        margin: 0 200px;

        .cards {
            display: flex;
            flex-direction: row;
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
            padding: 2rem 0;
 
            .card {
            width: 130px;
            height: 250px;
            background-color: aquamarine;
            margin: 1.5rem;
            text-align: center;
            }
        }
    }
}


</style>


