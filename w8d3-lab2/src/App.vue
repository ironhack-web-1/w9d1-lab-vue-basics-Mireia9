<template>
<div>
<NavBar></NavBar>
<p>{{2 + 2}}</p>
<FormContact></FormContact>
<FooterMain></FooterMain>
</div>
</template>

<script>
import NavBar from './components/NavBar.vue'
import FooterMain from './components/FooterMain.vue'
import FormContact from './components/FormContact.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    FooterMain,
    FormContact,
  }
}
</script>

<style>

</style>
