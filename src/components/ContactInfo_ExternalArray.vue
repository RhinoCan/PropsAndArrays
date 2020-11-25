<template>
    <!-- external data, simple array, no key -->
    <div class="Contact">
      <table>
          <tr v-for="contact_line in contact_lines_external_array" :key="contact_line"><td>{{ contact_line }}</td></tr>
      </table>
    </div>
</template>

<script>
export default {
  name: 'ContactInfo_ExternalArray',
  props: {
     contact_lines_external_array: { type: Array, required: false, default: () => ["Contact Data Pending"] }, //simple array
  },
  data() {
    return {
    }
  },
 created()  {
    console.log("Created " + this.Name);
  } 
 }
</script>  

<style scoped>
.Contact {
  margin-bottom: 20px;
  background-color: blueviolet;
  color: chartreuse;
}
td {
  line-height: 12px;
  font-family: sans-serif;
  text-align: left;
}
</style>
