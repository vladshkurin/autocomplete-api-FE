<template>
  <autocomplete
    url="http://localhost:3000/autocomplete"
    anchor="title"
    label="writer"
    :debounce="500"
    :on-select="getData">
  </autocomplete>

</template>


<script>

  import Autocomplete from 'vue2-autocomplete-js';

  export default {

    components: { Autocomplete },

    methods: {
      getData(obj){
        console.log(obj);
      }
    }
  };

</script>
