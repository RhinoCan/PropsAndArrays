<template>
    <!-- internal data, simple array, no key -->
    <div class="Contact">
      <table>
      <tr v-for="contact_line in contact_lines_internal_array" :key="contact_line"><td>{{ contact_line }}</td></tr>
      </table>
    </div>
</template>

<script>
export default {
  name: 'ContactInfo_InternalArray',
  data() {
    return {
      contact_lines_internal_array: [
        "456 Internal Array Street",
        "Toronto, ON",
        "H0H 0H0",
        "519 555 1212 [Phone]",
        "519 555 1212 [Fax]",
        "info@example.com" 
      ]
    }
  },
  created()  {
    console.log("Created " + this.name);
  }
 }
</script>  

<style scoped>
.Contact {
  margin-bottom: 20px;
  background-color: fuchsia;
}
td {
  line-height: 12px;
  font-family: sans-serif;
  text-align: left;
}
</style>
