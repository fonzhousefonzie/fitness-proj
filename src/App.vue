<template>
  <div id="app">
    <TheHeader/>
    <TheFooter/>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheFooter
}
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed&display=swap');

#app {
  font-family: 'Roboto Condensed', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 87px;
}

.primary-btn{
  background: #4154fe;
  padding: 0.5rem 1.5rem;
  color: white;
  border-radius: 2rem;
  font-size: 0.8rem;
  transition: background 300ms ease-out;
  &:hover{
    background: #ec5a57;
  }
}

.active{
  color: white;
}

.new::after{
  content: 'new';
  color: #060606;
  background: #fff941;
  margin-left: 0.5rem;
  padding: 0.2rem 0.3rem;
  font-size: 0.8rem;
  border-radius: 2px;
  font-weight: bold;
  vertical-align: middle;
}
</style>
