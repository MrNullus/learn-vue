# Dados nos Componentes

- Para isso usamos o `data` -> uma função que deve retornar um objeto com dados
- Podendo inicializar e modificar um valor na execução

Primeiro devemos criar o `data`:

```vue

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
```

Depois devemos utilizar dentro do template o dado que foi exportado:

```vue

<template>
  <h2>
    Usando dados no componente {{ dado }}
  </h2>
</template>
```

Se for feito isso temos um erro de sintaxe:

- Já que o template só aceita uma tag root, ou seja, devemos envolver o componenete com uma tag root

```vue

<template>
  <h2>
    Usando dados no componente {{ dado }}
  </h2>
  <p>
    Atualizando dados do componente...
  </p>
</template>
```

Deste modo, temos isto:

```vue

<template>
  <div>
    <h2>
      Usando dados no componente {{ dado }}
    </h2>
    <p>
      Atualizando dados do componente...
    </p>
  </div>
</template>
```
