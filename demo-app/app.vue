<template>
  <div>
    <h1>Hello World</h1>
    
    <Dummy />
    <h2 v-text="callGreeter()"></h2>
  </div>
</template>

<script lang="ts">
import Greeter from './utils/Greeter';

  export default {
    data() {
      return {
       
      }
    },
    methods: {
     callGreeter() {
      let num1: number;
      // num1 = 'asd';
      num1 = 22;
      
      let greet = new Greeter('From TS class');
      console.log(greet.greet());
      return greet.greet();
     }
    }
  }
</script>
