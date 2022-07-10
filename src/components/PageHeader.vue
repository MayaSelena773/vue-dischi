<template>
    <header>
        <!--Logo Header-->
        <img src="../assets/img/logo-spotify.png" alt="logo" class="small-logo">
    </header>
</template>

<script>
export default {
    name:'PageHeader'
}
</script>

<style lang="scss" scoped>
@import './style/vars.scss';

header {
    background-color: $brand_primary_color;
    width: 100%;
    height: 50px;

    .small-logo {
        width: 30px;
        margin: 0.5rem 1rem;
    }
}

</style>


