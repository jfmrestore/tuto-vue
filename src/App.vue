<template>
  <h1>Bonjour {{ firstName.toUpperCase() }}</h1>
  <p>Vous avez cliquer : {{ counter }} fois !</p>

  <p>Comment allez vous ?</p>
</template>
<script setup>
import {ref} from 'vue';
  const firstName="John";
  const counter = ref(1);
  setInterval(() =>  {counter.value++},1000  );
 

</script>
<style>
h1{
  color:red;
}
</style>