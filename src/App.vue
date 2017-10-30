var Scrollactive = require('vue-scrollactive');

<template>

  <div id="app">
    <div class="Title">Title</div>
      <nav>
      <ul>
        <li><a v-scroll-to="'#home'">Home</a></li>
        <li><a v-scroll-to="'#about'">About</a></li>
        <li><a v-scroll-to="'#comment'">Comment</a></li>
        <li><a v-scroll-to="'#menu'">Menu</a></li>
        <li><a v-scroll-to="'#gallery'">Gallery</a></li>
        <li><a v-scroll-to="'#contact'">Contact</a></li>
      </ul>
    </nav>
    <div id='home'><Intro/></div>
    <div id='about'><AboutUs/></div>
    <div id='comment'><CustomerComment/></div>
    <div id='menu'><Menu/></div>
    <div id='gallery'><Gallery/></div>
    <div id='contact'><FooterBar/></div>
  </div>
</template>

<script>

document.title = "Sushi Royal"
import Intro from './components/Intro'
import AboutUs from './components/AboutUs'
import CustomerComment from './components/CustomerComment'
import Menu from './components/Menu'
import Gallery from './components/Gallery'
import FooterBar from './components/FooterBar'

export default {
  name: 'app',
  components: {
    Intro,AboutUs,CustomerComment,Menu,Gallery,FooterBar
  },
  methods: {
       abc: function () {
$('html, body').animate({
        scrollTop: $(".test").offset().top
    }, 2000);
        }
      },
}


</script>

<style>

.Title {
  font-style: 'Arial';
  font-size: 120px;
  text-align: center
}

* {
  margin: 0;
  padding: 0;
}

nav {
  margin: 50px;
}

ul {
  overflow: auto;
  list-style-type: none;
}

li {
  height: 25px;
  float: left;
  margin-right: 0px;
  border-right: 1px solid #aaa;
  padding: 0 20px;
}

li:last-child {
  border-right: none;
}

li a {
  text-decoration: none;
  color: #ccc;
  font: 25px/1 Helvetica, Verdana, sans-serif;
  text-transform: uppercase;

  -webkit-transition: all 0.5s ease;
  -moz-transition: all 0.5s ease;
  -o-transition: all 0.5s ease;
  -ms-transition: all 0.5s ease;
  transition: all 0.5s ease;
}

li a:hover {
  color: #666;
}


</style>
