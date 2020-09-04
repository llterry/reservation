<template>
  <div id="app">
    <main>
      <div class="title">
        <Header />
      </div>
      <div class="calendar">
          <Calendar />
        </div>
        <div class="weekly">
          <Weekly />
        </div>
        <div class="button">
          <Button />
        </div>
        <div class="display">
          <Display />
        </div>
    </main>
  </div>

</template>

<script>
import Header from './components/Header';
import Calendar from './components/Calendar';
import Weekly from './components/Weekly';
import Button from './components/Button';
import Display from './components/Display';

export default {
  name: 'App',
  components: {
    Header,
    Calendar,
    Weekly,
    Button,
    Display
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'monserrat', sans-serif;
}

#app {
  background-image: url('./assets/cold-bg.jpg');
  background-size: cover;
  background-position: bottom;
  transition: 0.4s;
}

main {
  min-height: 100vh;
  padding: 25px;

  background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.25), rgba(0, 0, 0, 0.75));
}

.title {
  display: block;
  width: 100%;
  padding: 15px;
  margin-bottom: 35px;
  text-align: center;

  color: #313131;
  font-size: 30px;

  appearance: none; 
  border: none;
  outline: none;
  background: none;
}


/*
  box-shadow: 0px, 0px 8px rbga(0, 0, 0, 0.25);
  background-color: rgba(255, 255, 255, 0.5);
  border-radius: 0px, 16px, 0px, 16px;
  transition: 0.4s;
  */

</style>