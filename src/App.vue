<template>
  <AppHeader />

  <h1>{{ title }}</h1>
  <button
    @click="title = 'Hello World!'"
  >Нажми на меня</button>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
export default {
  components: {
    AppHeader
  },
  data() {
    return {
      title: 'Это тестовая страница'
    }
  }
}
</script>

<style scoped>

</style>
