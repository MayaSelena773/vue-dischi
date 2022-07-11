<template>

<div class="search flex">
    
    <input  
    type="text" 
    placeholder="Cerca il tuo album preferito">

    <label for="contacts-search">
        <i class="fa-solid fa-magnifying-glass my_glass"></i>
    </label>

</div>              
    
</template>

<script>
export default {
    name:'PageSearch'
}

</script>

<style lang="scss" scoped>
@import './style/vars.scss';

.search {
    background-color: $brand_secondary_color;
    padding-right: 20px;

    input {
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
    justify-content: flex-end;
}

</style>


