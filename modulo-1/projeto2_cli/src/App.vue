<template>
  <h1>
    Hello World
  </h1>

  <PrimeiroComponent/>
</template>

<script>
import PrimeiroComponent from "./components/PrimeiroComponent.vue";

export default {
  name : 'App',
  components : {
    PrimeiroComponent
  }
}
</script>