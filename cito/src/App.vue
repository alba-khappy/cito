<template>
  <div id="app">
    <heading />
    <breadcrumbs 
    v-bind:breadcrumbs="breadcrumbs"
    />
  </div>
</template>

<script>
import heading from '@/components/heading'
import breadcrumbs from '@/components/breadcrumbs'

export default {
  name: 'App',
  data() {
    return {
      breadcrumbs: [
        {id:1, title: 'Главная'},
        {id:2, title: 'Личный кабинет'},
        {id:3, title: 'Мои мероприятия'},
        {id:4, title: 'Создание мероприятия'}
      ]
    }
  },
  components: {
    heading,
    breadcrumbs
  }
}
</script>

<style>
#app {
  
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

</style>
