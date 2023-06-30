<template>
  <div>
    <h1>Hello World</h1>
    
    <Dummy />
    <h2 v-text="callGreeter()"></h2>
  </div>
</template>

<script>
import Greeter from './utils/Greeter';

  export default {
    data() {
      return {
       
      }
    },
    methods: {
     callGreeter() {
      let greet = new Greeter('From TS class');
      console.log(greet.greet());
      return greet.greet();
     }
    }
  }
</script>
