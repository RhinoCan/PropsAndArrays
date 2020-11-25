<template>
  <ContactInfo_ExternalArrayOfObjects :contact_lines_external_array_of_objects="contact_lines_external_array_of_objects"/>
</template>

<script>
import ContactInfo_ExternalArrayOfObjects from './components/ContactInfo_ExternalArrayOfObjects.vue';

export default {
  name: 'App',
  components: { ContactInfo_ExternalArrayOfObjects },
  data() {
    return {
      brand: 'Carrots Unlimited',
      proprietor: 'Bugs Bunny',
      contact_lines_external_array_of_objects: [
        { id: 1, content: "456 External Array of Objects Street" },
        { id: 2, content: "Toronto, ON" },
        { id: 3, content: "H0H 0H0" },
        { id: 4, content: "416 555 1212 [Phone]" },
        { id: 5, content: "905 555 1212 [Fax]" },
        { id: 6, content: "info@example.com" }
      ]
    }
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