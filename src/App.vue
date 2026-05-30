<template>
  <AppHeader />
  <!-- <h1>{{ title }}</h1>
  <button
    @click="title = 'Hello World!'"
  >Нажми на меня</button> -->
  <BaseForm />
  <BaseForm />
  <BaseForm />
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import BaseForm from './components/BaseForm.vue';
export default {
  components: {
    AppHeader,
    BaseForm
  },
  data() {
    return {
      title: 'Это тестовая страница'
    }
  }
}
</script>

<style>
  h1 {
    text-decoration: underline;
  }
</style>
