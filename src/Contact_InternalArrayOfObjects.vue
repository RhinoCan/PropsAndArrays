<template>
  <ContactInfo_InternalArrayOfObjects/>
</template>

<script>
import ContactInfo_InternalArrayOfObjects from './components/ContactInfo_InternalArrayOfObjects.vue';

export default {
  name: 'App',
  components: { ContactInfo_InternalArrayOfObjects },
  data() {
    return {
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