<template>
    <!-- internal data, array of objects with key -->
    <div class="Contact">
      <table>
        <tr v-for="contact_line in contact_lines_internal_array_of_objects" :key="contact_line.id">
          <td>{{ contact_line.content }}</td>
        </tr>
      </table>
    </div>
</template>

<script>
export default {
  name: 'ContactInfo_InternalArrayOfObjects',
   data() {
    return {
      contact_lines_internal_array_of_objects: [
        { id: 1, content: "456 Internal Array of Objects Street"},
        { id: 2, content: "Toronto, ON" },
        { id: 3, content: "H0H 0H0" },
        { id: 4, content: "519 555 1212 [Phone]" },
        { id: 5, content: "519 555 1212 [Fax]" },
        { id: 6, content: "info@example.com" }
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
  background-color: firebrick;
  color: white;
}
td {
  line-height: 12px;
  font-family: sans-serif;
  text-align: left;
}
</style>