<template>
  <div id="app">
    <TheHeader />
    <JumboTron />
    <CardsPrimaryBanner />
    <TheFooter />
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import JumboTron from './components/JumboTron.vue';
import CardsPrimaryBanner from './components/CardsPrimaryBanner.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheFooter,
    JumboTron,
    CardsPrimaryBanner
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Barlow+Semi+Condensed&display=swap');

#app {
  font-family: 'Barlow Semi Condensed', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}

button {
  border: none;
  outline: none;
  padding: 0.5em 1.5em;
  border-radius: 2rem;
  transition: background 300ms ease-out;
}

button.small {
  font-size: 0.8rem;
}

.primary-btn {
  background: #4154fe;
  color: white;

  &:hover {
    background: #ec5a57;
  }
}

.secondary-btn {
  background: #060606;
  color: #bcbcbc;
  border: 1px solid #78787a;

  &:hover {
    border: 1px solid white;
    background: white;
    color: #060606;
  }
}

.play-btn {
  padding: 1rem 1.4rem;
  color: #4154fe;
  transition: 200ms ease-out;

  &:hover {
    transform: scale(110%);
  }
}

.active {
  color: white;
}

.new::after {
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

.separator {
  width: 50px;
}

.separator-small {
  width: 30px;
}

.col-65 {
  width: 65%;
}

.col-30 {
  width: 30%;
}
</style>
