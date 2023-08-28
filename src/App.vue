<template>
  <Navbar></Navbar>
  <Hero></Hero>
  <Service></Service>
  <Produit></Produit>
  <Contact></Contact>
  <Footer></Footer>
</template>

<script >
import Navbar from './components/Navbar.vue';
import Hero from './components/Hero.vue';
import Service from './components/Service.vue';
import Produit from './components/Produit.vue';
import Contact from './components/Contact.vue';
import Footer from './components/Footer.vue';

export default{
  name: 'App',
  components:{
    Navbar,
    Hero,
    Service,
    Produit,
    Contact,
    Footer,
  }


}
</script>

<style >
@import './style.css';
</style>
