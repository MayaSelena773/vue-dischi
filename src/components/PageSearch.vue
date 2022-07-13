<template>

<div class="search flex">
    
    <select v-model="genre" @change="onClickLabel()">
        <option value="all">all</option>
        <option value="rock">rock</option>
        <option value="jazz">jazz</option>
    </select>

</div>              
    
</template>

<script>
export default {
    name:'PageSearch',
    data(){
        return {
            genre: ''
        }
    },
    methods: {
        onClickLabel() {
            this.$emit('changeGenre', this.genre);
        }
    }
};

</script>

<style lang="scss" scoped>
@import './style/vars.scss';

.search {
    background-color: $brand_secondary_color;
    padding-left: 110px;
    padding-top: 20px;

    select {
        padding: 10px;
        background-color: lightgreen;
    }

    .my_glass {
        font-size: 25px;
        padding-top: 7px;
        padding-left: 5px;
        color: white;
    }
}

.flex {
    display: flex;
    justify-content: flex-start;
}

</style>


