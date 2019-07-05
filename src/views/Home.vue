<template>
  <div>
    <p>{{ routeID }}</p>
    <p>{{ routeID2 }}</p>
    <!--: damit er weiß das eine Variable übergeben wird-->
    <HelloWorld :idUebergabe="routeID+' via Prop'"></HelloWorld>
  </div>
</template>
<script>
import HelloWorld from '@/components/HelloWorld.vue';
export default {
  components:{
    HelloWorld
  },
  data() {
    return {
      //Ausgabe: in der URL nach dem / (Slash)
      routeID: this.$route.params.id,
      routeID2: this.$route.params.andere

    };
  }
};
</script>
