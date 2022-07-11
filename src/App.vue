<template>
  <div id="app">
    <PageHeader />
    <PageSearch />
    <PageMain />
  </div>
</template>

<script>
import PageHeader from './components/PageHeader.vue';
import PageSearch from './components/PageSearch.vue';
import PageMain from './components/PageMain.vue';

export default {
  name: 'App',
  components: {
    PageHeader,
    PageSearch,
    PageMain
  }
}
</script>

<style lang="scss">
@import './components/style/common.scss';
</style>
