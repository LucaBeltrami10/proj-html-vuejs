<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  },
  data() {
    return {

    }
  },
  methods: {

  },

}
</script>


<style lang="scss">
@use '../src/style/general.scss' as *;
</style>