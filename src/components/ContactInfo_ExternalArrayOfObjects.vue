<template>
   <!-- external data, array of objects with key -->
   <div class="Contact">
      <table>
        <tr v-for="contact_line in contact_lines_external_array_of_objects" :key="contact_line.id"><td>{{ contact_line.content }}</td></tr>
      </table>
    </div>
</template>


<script>
export default {
  name: 'ContactInfo_ExternalArrayOfObjects',
  props: {
     contact_lines_external_array_of_objects: { type: Array, required: false, default: () => [{ id: 0, content: "Still waiting for info" }] }, //array of objects
  },
  data() {
    return {
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
  background-color: goldenrod;
  color: navy;
}
td {
  line-height: 12px;
  font-family: sans-serif;
  text-align: left;
}
</style>