<template>
  <AppHeader :headerNavEl="headerNavEl" />
  <AppMain />
  <AppFooter :footerListEl="footerListEl" />
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
      headerNavEl: [
        {
          element: 'Home',
          options: false
        },
        {
          element: 'About Us',
          options: false
        },
        {
          element: 'Trainings',
          options: ['Riding Lesson', 'Safe Drive', 'Mountain Bike', 'Trail Drive', 'Pedaling', 'All Trainings'],
        },
        {
          element: 'Packages',
          options: false
        },
        {
          element: 'Blog',
          options: false
        },
        {
          element: 'Contact',
          options: false
        },
      ],
      footerListEl: [
        {
          listName: 'Trainigns',
          options: ['Riding Lesson', 'Safe Drive', 'Mountain Bike', 'Trail Drive', 'Pedaling']
        },
        {
          listName: 'Quick Links',
          options: ['Home', 'About Us', 'Blog', 'Packages', 'Contact']
        }

      ]

    }
  },
  methods: {

  },

}
</script>


<style lang="scss">
@use '../src/style/general.scss' as *;
</style>