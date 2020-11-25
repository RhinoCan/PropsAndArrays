<template>
  <ContactInfo_ExternalArray :contact_lines_external_array="contact_lines_external_array"/>
</template>

<script>
import ContactInfo_ExternalArray from './components/ContactInfo_ExternalArray.vue';

export default {
  name: 'App',
  components: { ContactInfo_ExternalArray },
  data() {
    return {
      brand: 'Carrots Unlimited',
      proprietor: 'Bugs Bunny',
      contact_lines_external_array: [
        "456 External Array Street",
        "Toronto, ON",
        "H0H 0H0",
        "416 555 1212 [Phone]",
        "905 555 1212 [Fax]",
        "info@example.com"
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