<template>
  <!-- <div id="createEvent" v-bind:style="{ backgroundColor:'#FFF0C8'}"> -->
  <h1>Create New Event</h1>
  <p>Event Type:</p>
  <p>Event Name:</p>
  <v-btn elevation="2">Button</v-btn>
</template>

<script>
// import Dropdown from 'vue-simple-search-dropdown';
export default {
  name: 'CreateEvent',
  beforeCreate () {
    document.querySelector('body').setAttribute('style', 'background:#FFF0C8')
  },
  beforeUnmount () {
    document.querySelector('body').setAttribute('style', '')
  },
  components: {
      // Dropdown
  }
}
// document.body.style.backgroundColor = 'FFF0C8';
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Ubuntu&display=swap');
h1 {
  font-family:'Roboto', sans-serif;
  /* font-weight:300; */
  font-size:3em;
  color:#EC602D;
  -webkit-text-stroke-width: 1px;
  -webkit-text-stroke-color: black;
}
p {
  font-family:'Roboto', sans-serif;
}
</style>