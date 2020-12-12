<template>
  <div id="app">
    <b-img
      src="./assets/pete.jpg"
      rounded
      width="200px"
      alt="Photo of Purdue Pete"
    ></b-img>

    <h1>Purdue Pete</h1>
    <p>
      Hello, my name is Pete, and I am a computer science student at Purdue
      University.
    </p>

    <SocialLinks />

    <Projects />

    <ContactForm />
  </div>
</template>

<script>
import ContactForm from "./components/ContactForm";
import Projects from "./components/Projects";
import SocialLinks from "./components/SocialLinks";

export default {
  components: {
    ContactForm,
    Projects,
    SocialLinks,
  },
};
</script>

<style>
#app {
  text-align: center;
  margin: 50px;
}

#app h2 {
  margin-top: 1em;
}
</style>
