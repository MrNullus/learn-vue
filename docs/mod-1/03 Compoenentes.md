# Componentes
Assim como em outras ferraentas a base das interfaces são **componentes**;
Já que com eles ganhamos uma baixa complexidade na hora de fazer manutenção já que eles estão separados por responsabilidade.

Alem de que com a componentiação no vue teremos um CSS por escopo (reflete apenas no componente) além de que teremos determinados dados de cada componente

## Começo
É com a tag `template` que colocamos o que será exibido na página

> Ou seja, é a nossa parte visual

- Criamos então o componente:
```vue
<template>
  <h1>
    Hello World
  </h1>
</template>
```

- Agora devemos exporta-lo:
```vue
<script>
export default {
  name: 'App'
}
</script>
```
> Observe que para exportar usamos uma tag script no mesmo arquivo e perceeba que passamos `name` -> se atente já que esse será o nome do compoenete que será exportado, logo devemos usar o mesmo nome que está ali criado