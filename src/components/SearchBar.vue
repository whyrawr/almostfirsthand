<template>
  <div class="searchBar">
      <input v:on-click="hello" class="searchBar__input" type="text">
      <ul class="searchBar__response">
        <li class="response__item">List Item</li>
        <li class="response__item">List Item</li>
        <li class="response__item">List Item</li>
        <li class="response__item">List Item</li>
      </ul>
  </div>
</template>

<script>
export default {
  name: 'SearchBar',
  data() {
    return{

    }
  },
  hello() {
    console.log('Hello!');
  }
}
</script>

<style>
.searchBar {
  position: relative;
}

.searchBar__input {
  box-sizing: border-box;

  width: 750px;
  height: 55px;

  border: 1px solid #000;
  padding: 10px;

  outline: none;

  font-size: 24px;
}

.searchBar__response {
  position: absolute;
  top: 55px;
  left: 0;
  right: 0;

  list-style: none;
  padding: 0;
  margin: 0;
}

.response__item {
  padding: 10px;
  font-size: 18px;
}

.response__item:hover {
  cursor: pointer;
  background-color: rgba(0,0,0,.1);
}
</style>
