<script>
export default {
  name : "PrimeiroComponent",
  data() {
    return {
      dado : "jogando dados no compoente",
    }
  }
}
</script>

<template>
  <h2>
    Usando dados no componente {{ dado }}
  </h2>
  <p>
    Atualizando dados do componente...
  </p>
</template>

<style scoped>

</style>