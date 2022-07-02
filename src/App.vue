<template>
  <div id="app">
    <TheHeader />
    <JumboTron />
    <CardsPrimaryBanner />
    <YoutubeSection />
    <FeaturedSection/>
    <MailingList/>
    <BlueCardsBanner/>
    <LatestSection/>
    <TheFooter />
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import JumboTron from './components/JumboTron.vue';
import CardsPrimaryBanner from './components/CardsPrimaryBanner.vue';
import YoutubeSection from './components/YoutubeSection.vue';
import FeaturedSection from './components/FeaturedSection.vue';
import MailingList from './components/MailingList.vue';
import BlueCardsBanner from './components/BlueCardsBanner.vue';
import LatestSection from './components/LatestSection.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheFooter,
    JumboTron,
    CardsPrimaryBanner,
    YoutubeSection,
    FeaturedSection,
    MailingList,
    BlueCardsBanner,
    LatestSection
}
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Barlow+Semi+Condensed&display=swap');

:root {
  --blue: #4154fe;
  --yellow: #fff941;
  --red: #ec5a57;
  --lighter-red: #f78280;
  --black: #060606;
  --light-grey: #bcbcbc;
  --dark-grey: #78787a;
  --darker: #a00644;
  --lighter: #b6967e;
}

#app {
  font-family: 'Barlow Semi Condensed', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}

h1 {
  font-size: 4.7rem;
  font-weight: bold;
}

h2 {
  font-size: 3rem;
}

h5 {
  font-size: 1.7rem;
}

h6 {
  font-size: 1.45rem;
}

a{
  text-decoration: none;
  color: inherit;
  &:hover{
    color: var(--blue);
  }
}

button {
  border: none;
  outline: none;
  padding: 0.7em 1.7em;
  border-radius: 2rem;
  font-size: 1.3rem;
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

.tertiary-btn{
  background: red;
  color: white;
  &:hover{
    background: var(--red);
  }
}

.play-btn {
  aspect-ratio: 1 / 1;
  padding: 1.4rem 1.9rem;
  border-radius: 50%;
  color: #4154fe;
  transition: 200ms ease-out;

  &:hover {
    transform: scale(110%);
  }
}

.play-btn.small{
  padding: 1rem 1.3rem 1rem 1rem;
}

input[type="email"]{
  border: none;
  outline: none;
  padding: 1.2em 1.7em;
  border-radius: 3rem;
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
}

.separator {
  width: 70px;
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

.col-50{
  width: 50%;
}

.c-b-radius {
  border-radius: 0.3rem 0.3rem 3rem;
}
</style>
