<template>
  <div id="app">
    <app-nav-bar/>
    <app-header/>
    <app-services/>
    <app-products/>
    <app-about/>
    <app-team/>
    <app-clients/>
    <app-contacts/>
    <app-footer/>
    <app-modal/>
  </div>
</template>

<script>
import Navbar from './components/Navbar';
import Header from './components/Header';
import Services from './components/Services';
import Products from './components/Products';
import About from './components/About';
import Teams from './components/Teams';
import Clients from './components/Clients';
import Contacts from './components/Contacts';
import Footer from './components/Footer';
import Modal from './components/Modal';

export default {
  name: 'App',
  components: {
    appNavBar: Navbar,
    appHeader: Header,
    appServices: Services,
    appProducts: Products,
    appAbout: About,
    appTeam: Teams,
    appClients: Clients,
    appContacts: Contacts,
    appFooter: Footer,
    appModal: Modal
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
  margin-top: 60px;
}
</style>
