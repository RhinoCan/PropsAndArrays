<template>
  <ContactInfo_InternalArray/>
</template>

<script>
import ContactInfo_InternalArray from './components/ContactInfo_InternalArray.vue';

export default {
  name: 'App',
  components: { ContactInfo_InternalArray },
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