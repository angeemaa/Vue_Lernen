<template>
  <div>
    <p>{{ routeID }}</p>
    <p>{{ routeID2 }}</p>

  </div>
</template>
<script>
export default {
  data() {
    return {
      //Ausgabe: in der URL nach dem / (Slash) 
      routeID: this.$route.params.id, 
      routeID2: this.$route.params.andere 

    };
  }
};
</script>
