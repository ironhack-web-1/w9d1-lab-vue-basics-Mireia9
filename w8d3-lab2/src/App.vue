<template>
  <div>
    <NavBar></NavBar>
    <p>{{ 2 + 2 }}</p>
    <FormContact></FormContact>
    <hr />
    <div v-if="DayOfClass === `true`">
      Today you have class in Ironhack, connect your computer!!!
    </div>
    <div v-else>Day off, go for a ride</div>
    <hr />
    <PostBloc></PostBloc>
    <FooterMain></FooterMain>
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import FooterMain from "./components/FooterMain.vue";
import FormContact from "./components/FormContact.vue";
import PostBloc from "./components/PostBloc.vue";

export default {
  name: "App",
  data() {
    return {
      DayOfClass: "true",
    };
  },
  components: {
    NavBar,
    FooterMain,
    FormContact,
    PostBloc
},
};
</script>

<style></style>
