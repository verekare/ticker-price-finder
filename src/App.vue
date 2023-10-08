<template>
<TickerForm />
<TickerList />
</template>
 
<script>
import TickerForm from './components/TickerForm.vue'
import TickerList from './components/TickerList.vue'
import TickerItem from './components/TickerItem.vue'

export default {
  components: {
    TickerForm, TickerList, TickerItem
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
}
</style>
