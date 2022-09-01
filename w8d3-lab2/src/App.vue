<template>
  <div>
    <NavBar />
    <p>{{ 2 + 2 }}</p>
    <FormContact />
    <hr />
    <div v-if="DayOfClass === `true`">
      Today you have class in Ironhack, connect your computer!!!
    </div>
    <div v-else>Day off, go for a ride</div>
    <hr />
    <PostBloc />
    <hr />
    <NewForm v-model="newName" placeholder="Su Nombre"/>
    <NewForm v-model="newMail" placeholder="Su email" type="email"/>
    <p>Mi nombre és: {{ newName }}</p>
    <p>Mi e-mail és: {{ newMail }}</p>
    <hr />
    <FooterMain />
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import FooterMain from "./components/FooterMain.vue";
import FormContact from "./components/FormContact.vue";
import PostBloc from "./components/PostBloc.vue";
import NewForm from "./components/NewForm.vue";

export default {
  name: "App",
  data() {
    return {
      DayOfClass: "true",
      newName: null,
      newMail: null,
      };
  },
  components: {
    NavBar,
    FooterMain,
    FormContact,
    PostBloc,
    NewForm,
  },
};
</script>

<style></style>
