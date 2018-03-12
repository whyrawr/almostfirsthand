<template>
  <div class="index">
    <SearchBar></SearchBar>
  </div>
</template>

<script>
import SearchBar from './SearchBar'

export default {
  name: 'Index',
  components: {
    SearchBar,
  },

  data() {
    return{
      msg: ''
    }
  }
}
</script>

<style>
  .index {
    
  }
</style>